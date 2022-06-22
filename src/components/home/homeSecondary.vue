<template>
    <section id="secondary-banner">
        <div class="secondary-text">
          <div class="wrapper">
          <h2>Emphasis on People and Planet</h2>
          <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. 
            Aliquid odit perferendis. accusamus assumenda et quasi beatae sunt totam atque vel!</p>
          <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. 
          Aliquid odit perferendis. accusamus assumenda et quasi beatae sunt totam atque vel!</p>
          <a href="">Read more</a>
          </div>   
        </div>
    </section>
</template>

<style scoped>
  #secondary-banner {
  background-image: url('@/assets/88322.webp');
  background-repeat: no-repeat;
  background-attachment: fixed;
  background-position: center;
  background-size: cover;
  position: relative;
  padding: 8.5rem 0rem;
}


.secondary-text {
  width: 100%;
  max-width: 1200px;
  height: 100%;
  margin: 0px auto;
  padding: 0px 1.2rem;
}

.secondary-text .wrapper {
 background: #fff;
 width: 557px;
 padding: 65px;
 border-radius: 10px;
 position: relative;
}

.secondary-text h2 {
  font-size: 2.4rem;
  font-family: 'Lora', serif;
  margin-bottom: 20px;
}

.secondary-text p {
  margin: 10px 0px;
  font-size: 0.95rem;
  font-weight: 300;
}


.secondary-text a {
  display: inline-block;
  font-size: 0.9rem;
  background: fff;
  padding: 12px 32px;
  text-transform: uppercase;
  text-decoration: none;
  font-weight: 500;
  margin-top: 30px;
  background-color: #262626;
  color: #fff;
  border-radius: 30px;
  letter-spacing: 2px;
}

.secondary-text a:hover {
  background: #dc3d04;
  color: #fff;
}

@media only screen and (max-width: 1024px) {
  .secondary-text .wrapper { 
    width: 475px;
    padding: 50px 65px;
  }



}

@media only screen and (max-width: 768px) {
   .secondary-text .wrapper { 
    width: 100%;
    top: 140px;
    padding: 45px 50px;;
}

 #secondary-banner {
  padding: 12rem 0rem;
 }

.secondary-text h2 {
 font-size: 2rem;
}

}

@media only screen and (max-width: 576px) {
  .secondary-text h2 {
 font-size: 1.7rem;
}

.secondary-text p {
 
  font-size: 0.9rem;
  
}

.secondary-text a {
  font-size: 0.8rem;
    padding: 12px 31px;
}


   .secondary-text .wrapper { 
 
    padding: 40px;
}



}


@media only screen and (max-width: 380px) {
    .secondary-text h2 {
 font-size: 1.6rem;
}

.secondary-text p {
 
  font-size: 0.85rem;
  
}

.secondary-text a {
  padding: 12px 25px;
  font-size: 0.75rem;
  margin-top: 15px;
}

   .secondary-text .wrapper { 
    width: 100%;
    top: 150px;
   }


}


  @media (max-width: 335px) {
       .secondary-text h2 {
     font-size: 1.3rem;
   }
  }



</style>