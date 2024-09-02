<template>
  <div class="fixed top-0 left-0 w-full h-screen">
    <!-- Container for the 3D model -->
    <div ref="container" class="w-full h-full"></div>
  </div>
</template>

<script setup>
import { onMounted, ref } from 'vue';
import * as THREE from 'three';
import { GLTFLoader } from 'three/examples/jsm/loaders/GLTFLoader.js';
import gsap from 'gsap';
import { ScrollTrigger } from 'gsap/ScrollTrigger';

gsap.registerPlugin(ScrollTrigger);

const container = ref(null);

onMounted(() => {
  // Setup basic Three.js scene
  const scene = new THREE.Scene();

  const camera = new THREE.PerspectiveCamera(70, window.innerWidth / window.innerHeight, 0.2, 1000);
  const renderer = new THREE.WebGLRenderer({ antialias: true });
  renderer.setSize(window.innerWidth, window.innerHeight);
  container.value.appendChild(renderer.domElement);

  // Add lighting to the scene
  const light = new THREE.DirectionalLight(0xffffff, 10);

  scene.add(light);




  // Load the GLB model
  const loader = new GLTFLoader();
  loader.load('/spiderman.glb', function (gltf) {
    const model = gltf.scene;
   
    scene.add(model);

    // Initial model scale and position
    model.scale.set(3, 3, 3); // Increase the scale
    model.position.set(9,-7, 1); // Position the model to the right side

   

    // Set initial camera position
    camera.position.set(4, 2, -3); // Adjust camera position
    camera.lookAt(camera.position); // Ensure camera is looking at the model

    // Animation loop
    function animate() {
      requestAnimationFrame(animate);
      renderer.render(scene, camera);
    }
    animate();

    // Use GSAP to animate the model and camera on scroll
    ScrollTrigger.create({
      trigger: document.body,
  
      scrub: true,
      onUpdate: (self) => {
        const progress = self.progress;
       

        // Rotate the model around the Y-axis based on scroll progress
        model.rotation.y = 1 +(progress * Math.PI * 5);

        // Adjust camera position based on scroll
        camera.position.z = 8 - progress * 3; // Zoom effect
        camera.position.y = 2 + progress * 2; // Slight vertical movement
        camera.position.x = 6 + progress * 1; // Move camera to keep model in view

        // Ensure the camera is always looking at the model
        camera.lookAt(camera.position);
     

        // Log model position during scroll
        console.log('Model position during scroll:', model.position);
        fog.near = 10 + progress * 10; // Animate the fog near distance
        fog.far = 50 - progress * 30;   // Animate the fog far distance

        // Adjust light position
        light.position.set(
          Math.sin(progress * Math.PI * 2) * 4,
          10,
          Math.cos(progress * Math.PI * 2) * 3
        );
      }
    });
  }, undefined, function (error) {
    console.error(error);
  });

  // Handle window resize
  window.addEventListener('resize', () => {
    camera.aspect = window.innerWidth / window.innerHeight;
    camera.updateProjectionMatrix();
    renderer.setSize(window.innerWidth, window.innerHeight);
  });
});
</script>

<style scoped>
/* Ensures the container covers the full viewport and is fixed in place */
.fixed {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100vh;
  z-index: 10;
}
</style>
