<template>
  <header id="showcase">
     <video src="../../assets/banana.mp4" muted loop autoplay></video>
     <div class="overlay"></div>
     <div class="text">
          <h2>{{ videoTitle }}</h2>
           <p>{{ videoSubTitle }}</p>
          <button @click="scrollDown">{{ videoButton }}</button>
     </div> 
   </header>
</template>

<script>
   export default {
     props: ["videoTitle", "videoSubTitle", "videoButton"],
     methods: {
       scrollDown() {
         const height = document.querySelector('#nav').offsetHeight;
         this.gsap.to(window, {duration: 1, scrollTo: {y: "#main-container", offsetY: height}});
       }
     }
   }
</script>

<style scoped>

  #showcase {
  position: relative;
  right: 0;
  width: 100%;
  min-height: 100vh;
  display: flex;
  justify-content: space-between;
  align-items: center;
  background: #111;
  transition: 0.5s;
  z-index: 0;
}

#showcase video {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  object-fit: cover;
  opacity: 0.8;
  z-index: 0;
}

.overlay {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: #00000059;
  mix-blend-mode: overlay;
}

.text {
  max-width: 1200px;
  padding: 1.2rem;
  width: 100%;
  margin: 3rem auto 0rem auto;
  z-index: 10;
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  text-align: left;
}

.text h2 {
  font-size: 3.8rem;
  font-weight: 800;
  color: #fff;
  text-align: left;
  line-height: 1em;
  text-transform: uppercase;
}

.text p {
  font-size: 1.1em;
  color: #fff;
  margin: 20px 0;
  font-weight: 400;
}

.text button {
  border: none;
  display: inline-block;
  font-size: 1em;
  background: #fff;
  padding: 10px 30px;
  text-transform: uppercase;
  text-decoration: none;
  font-weight: 500;
  margin-top: 10px;
  color: #111;
  border-radius: 20px;
  letter-spacing: 2px;
  transition: 0.3s;
  font-family: 'Poppins', sans-serif;
}
.text button:hover
{
  background: #dc3d04;
  color: #fff;
}


  @media (min-width: 481px) and (max-width: 767px) {
  .text h2 {
     font-size: 3rem;
   }
  .text p {
    font-size: 1rem;
    margin: 15px 0px;
   }

   .text button {
     font-size: 0.9em;
     padding: 10px 25px;
     margin-top: 0;
   }
 }

 @media (min-width: 376px) and (max-width: 480px) {
    .text h2 {
     font-size: 2.3rem;
   }
     .text p {
    font-size: 0.9rem;
     margin: 15px 0px;
  
   }

   .text button {
     font-size: 0.8em;
     padding: 10px 20px;
     margin-top: 0;
   }
  }

  @media (max-width: 375px) {

    .text h2 {
     font-size: 2rem;
   }
     .text p {
    font-size: 0.85rem;
     margin: 15px 0px;
   }

   .text button {
     font-size: 0.75em;
     padding: 10px 20px;
     margin-top: 0;
   }
  }
 

</style>


