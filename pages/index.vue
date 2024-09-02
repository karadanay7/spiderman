<template>
  <div class="relative  bg-black">
    
    <!-- Spiderman Component with fixed positioning -->
    <div class="fixed top-0  w-full h-screen z-10 ">
      <Spiderman />
    </div>
    <div class=" fixed top-16 left-24 w-full z-30  "> <img src="/header.png" alt=""></div>

    <!-- Main Content with Scroll Effect -->
    <div class=" flex flex-col justify-between relative p-4  z-20"> 
      <!-- Content on the first page -->
      <div class="min-h-screen flex items-center justify-start text-white  relative w-full ml-20">
        <div class="text-start ">
          <iframe width="560" height="315" src="https://www.youtube.com/embed/e5wUilOeOmg?si=h9Pe7q65ltO-x8FS" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
          <h1 class="text-3xl font-extrabold mb-4">SPIDERMAN 3: THE DARK SIDE OF HEROISM</h1>
          <p class="text-xl mb-8 italic">"Every hero has a dark side. Discover the untold story."</p>
          <a href="#second-page" class="bg-red-600 hover:bg-red-700 text-white px-8 py-4 rounded-lg text-2xl font-semibold transition">Enter the Darkness</a>
        </div>
      </div>
      

      <!-- Content on the second page -->
      <div id="second-page" class="min-h-screen flex flex-col items-start justify-center text-white relative   gap-20 ">
        <div class="flex flex-col items-center  self-start">
          
     
      <h2 class="font-index italic text-5xl linear-wipe-hero  font-bold text-start  -ml-12">GREATEST BATTLE LIES WITHIN.</h2>
    

    <div class="max-w-[700px] bg-black text-white  bg-opacity-10 rounded-lg font-index ml-20 mt-20 animate-fade text-lg">
      <h3 class="text-xl font-semibold mb-2">Peter Parker (Tobey Maguire)</h3>
      <p class=" mb-4">
        Finally has the girl of his dreams, Mary Jane Watson (Kirsten Dunst), and New York City is in the throes of Spider-mania! But when a strange alien symbiote turns Spider-Man's suit black, his darkest demons come to light changing Spider-Man inside as well as out.
      </p>
      <p class=" mb-4">
        Spider-Man is in for the fight of his life against a lethal mix of villains - the deadly Sandman (Thomas Haden Church), Venom (Topher Grace), and the New Goblin (James Franco) - as well as the enemy within himself.
      </p>
     
    </div>
        </div>
          <div class="flex   gap-10 ml-20">
            <a href="http://bit.ly/SonyPicsSubscribe" class="text-3xl hover:text-red-600" target="_blank" rel="noopener noreferrer">
              <svg xmlns="http://www.w3.org/2000/svg" width="2.86em" height="2em" viewBox="0 0 256 180"><path fill="#f00" d="M250.346 28.075A32.18 32.18 0 0 0 227.69 5.418C207.824 0 127.87 0 127.87 0S47.912.164 28.046 5.582A32.18 32.18 0 0 0 5.39 28.24c-6.009 35.298-8.34 89.084.165 122.97a32.18 32.18 0 0 0 22.656 22.657c19.866 5.418 99.822 5.418 99.822 5.418s79.955 0 99.82-5.418a32.18 32.18 0 0 0 22.657-22.657c6.338-35.348 8.291-89.1-.164-123.134"/><path fill="#fff" d="m102.421 128.06l66.328-38.418l-66.328-38.418z"/></svg>
            </a>
            <a href="https://www.facebook.com/sonypictureshomeentertainment" class="text-3xl hover:text-red-600" target="_blank" rel="noopener noreferrer">
              <svg xmlns="http://www.w3.org/2000/svg" width="2em" height="2em" viewBox="0 0 256 256"><path fill="#1877f2" d="M256 128C256 57.308 198.692 0 128 0S0 57.308 0 128c0 63.888 46.808 116.843 108 126.445V165H75.5v-37H108V99.8c0-32.08 19.11-49.8 48.348-49.8C170.352 50 185 52.5 185 52.5V84h-16.14C152.959 84 148 93.867 148 103.99V128h35.5l-5.675 37H148v89.445c61.192-9.602 108-62.556 108-126.445"/><path fill="#fff" d="m177.825 165l5.675-37H148v-24.01C148 93.866 152.959 84 168.86 84H185V52.5S170.352 50 156.347 50C127.11 50 108 67.72 108 99.8V128H75.5v37H108v89.445A129 129 0 0 0 128 256a129 129 0 0 0 20-1.555V165z"/></svg>
            </a>
            <a href="https://www.instagram.com/sonypictureshomeentertainment" class="text-3xl hover:text-red-600" target="_blank" rel="noopener noreferrer">
           <svg xmlns="http://www.w3.org/2000/svg" width="2em" height="2em" viewBox="0 0 256 256"><g fill="none"><rect width="256" height="256" fill="url(#skillIconsInstagram0)" rx="60"/><rect width="256" height="256" fill="url(#skillIconsInstagram1)" rx="60"/><path fill="#fff" d="M128.009 28c-27.158 0-30.567.119-41.233.604c-10.646.488-17.913 2.173-24.271 4.646c-6.578 2.554-12.157 5.971-17.715 11.531c-5.563 5.559-8.98 11.138-11.542 17.713c-2.48 6.36-4.167 13.63-4.646 24.271c-.477 10.667-.602 14.077-.602 41.236s.12 30.557.604 41.223c.49 10.646 2.175 17.913 4.646 24.271c2.556 6.578 5.973 12.157 11.533 17.715c5.557 5.563 11.136 8.988 17.709 11.542c6.363 2.473 13.631 4.158 24.275 4.646c10.667.485 14.073.604 41.23.604c27.161 0 30.559-.119 41.225-.604c10.646-.488 17.921-2.173 24.284-4.646c6.575-2.554 12.146-5.979 17.702-11.542c5.563-5.558 8.979-11.137 11.542-17.712c2.458-6.361 4.146-13.63 4.646-24.272c.479-10.666.604-14.066.604-41.225s-.125-30.567-.604-41.234c-.5-10.646-2.188-17.912-4.646-24.27c-2.563-6.578-5.979-12.157-11.542-17.716c-5.562-5.562-11.125-8.979-17.708-11.53c-6.375-2.474-13.646-4.16-24.292-4.647c-10.667-.485-14.063-.604-41.23-.604zm-8.971 18.021c2.663-.004 5.634 0 8.971 0c26.701 0 29.865.096 40.409.575c9.75.446 15.042 2.075 18.567 3.444c4.667 1.812 7.994 3.979 11.492 7.48c3.5 3.5 5.666 6.833 7.483 11.5c1.369 3.52 3 8.812 3.444 18.562c.479 10.542.583 13.708.583 40.396s-.104 29.855-.583 40.396c-.446 9.75-2.075 15.042-3.444 18.563c-1.812 4.667-3.983 7.99-7.483 11.488c-3.5 3.5-6.823 5.666-11.492 7.479c-3.521 1.375-8.817 3-18.567 3.446c-10.542.479-13.708.583-40.409.583c-26.702 0-29.867-.104-40.408-.583c-9.75-.45-15.042-2.079-18.57-3.448c-4.666-1.813-8-3.979-11.5-7.479s-5.666-6.825-7.483-11.494c-1.369-3.521-3-8.813-3.444-18.563c-.479-10.542-.575-13.708-.575-40.413s.096-29.854.575-40.396c.446-9.75 2.075-15.042 3.444-18.567c1.813-4.667 3.983-8 7.484-11.5s6.833-5.667 11.5-7.483c3.525-1.375 8.819-3 18.569-3.448c9.225-.417 12.8-.542 31.437-.563zm62.351 16.604c-6.625 0-12 5.37-12 11.996c0 6.625 5.375 12 12 12s12-5.375 12-12s-5.375-12-12-12zm-53.38 14.021c-28.36 0-51.354 22.994-51.354 51.355s22.994 51.344 51.354 51.344c28.361 0 51.347-22.983 51.347-51.344c0-28.36-22.988-51.355-51.349-51.355zm0 18.021c18.409 0 33.334 14.923 33.334 33.334c0 18.409-14.925 33.334-33.334 33.334s-33.333-14.925-33.333-33.334c0-18.411 14.923-33.334 33.333-33.334"/><defs><radialGradient id="skillIconsInstagram0" cx="0" cy="0" r="1" gradientTransform="matrix(0 -253.715 235.975 0 68 275.717)" gradientUnits="userSpaceOnUse"><stop stop-color="#fd5"/><stop offset=".1" stop-color="#fd5"/><stop offset=".5" stop-color="#ff543e"/><stop offset="1" stop-color="#c837ab"/></radialGradient><radialGradient id="skillIconsInstagram1" cx="0" cy="0" r="1" gradientTransform="matrix(22.25952 111.2061 -458.39518 91.75449 -42.881 18.441)" gradientUnits="userSpaceOnUse"><stop stop-color="#3771c8"/><stop offset=".128" stop-color="#3771c8"/><stop offset="1" stop-color="#60f" stop-opacity="0"/></radialGradient></defs></g></svg>
            </a>
            <a href="https://twitter.com/sonypicshomeent" class="text-3xl hover:text-red-600" target="_blank" rel="noopener noreferrer">
              <svg xmlns="http://www.w3.org/2000/svg" width="2em" height="2em" viewBox="0 0 16 16"><path fill="currentColor" d="M12.6.75h2.454l-5.36 6.142L16 15.25h-4.937l-3.867-5.07l-4.425 5.07H.316l5.733-6.57L0 .75h5.063l3.495 4.633L12.601.75Zm-.86 13.028h1.36L4.323 2.145H2.865z"/></svg>
            </a>
          </div>
       
      
      </div>
    </div>
  </div>
</template>

<script setup>

</script>

<style scoped>
/* Ensure content is not covered by Spiderman component */
section {
  position: relative;
  z-index: 20;
  /* Ensure content is above the Spiderman component */
}
.linear-wipe-hero{
  
  
  background: linear-gradient(to right, #ebebf0 20%, rgb(172, 35, 35) 40%, rgb(28, 27, 27) 60%, #000000 80%);
  background-size: 200% auto;
  
  color: #000;
  background-clip: text;

  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  
  animation: shine 3s linear infinite;
  @keyframes shine {
    to {
      background-position: 200% center;
    }
  }

}




/* Additional styling if needed */
</style>
