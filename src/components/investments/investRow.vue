<template>

  <section id="about-rows">
       <div class="row">
          <div class="left-row image"></div>
           <div class="right-row">
              <div class="right-text">
                 <h3>Moyee Ethiopia</h3>
                 <h5>Leading coffee company in Ethiopia</h5>
                 <p>Moyee Coffee PLC is quickly becoming the first multi-national coffee company based out of Ethiopia. 
                   They have managed to become the first ISO certificated Coffee Roaster in Ethiopia, with revolutionary fairchain
                   practices such as world-class roasting and packaging facilities and living wages. Moyee has also sold over 5 million cups of Fairtraide coffee in 2019.
                   The company is Further growing in Ethiopia and other African coffee drinking growth market, while also launching new brands.</p>
                 <a class="btn" href="#">Visit site</a>
              </div>
          </div>
       </div>  
       <div class="row-reverse">
          <div class="left-row2 image"></div>
           <div class="right-row">
              <div class="right-text">
                 <h3>AgroFair</h3>
                 <h5>Fairtrade organic fruit</h5>
                 <p> AgroFair is a true market pioneer in producing and importing fairtrade fruit, such as bananas, banana paste and sweet potatoes.
                  The company has been a frontrunner in Europe, and it is located at the world's biggest importer of bananas with a large marketshare.
                  Our goal with AgroFair is to promote equal opportunities for male and female workers, 
                  monitoring pesticides, improving watermanagement and healthy soils. Animal welfare will be our focus as well.</p> 
                 <a class="btn" href="#">Visit site</a>          
              </div>
          </div>
       </div>  
       
  </section>
  
</template>

<style scoped>
  .row{
    width: 100%;
    max-width: 1200px;
    margin: 3rem auto 6.5rem auto;
    padding: 0rem 1.2rem;
    display: flex;
    align-items: center;
  }

  .left-row {
    background: url("@/assets/Moyee.webp");
    background-size: cover;
    background-repeat: no-repeat;
    background-position: center;
    width: 45%;
    height: 520px;
  }

  .right-row {
    width: 55%;
    background: #fff;
    padding: 40px;
    box-shadow: rgb(0 0 0 / 8%) 0px 0px 30px 0px;
    display: flex;
    margin-left: -100px;
  }


 h3{
   display: inline-block;
   font-size: 1.65rem;
   font-family: 'Lora', serif;
 }

 h5 {
    margin: 0.55rem 0rem;
    font-size: 1.15rem;
    font-weight: 500;
     font-family: 'Lora', serif;
 }

 p {
   font-weight: 300;
   font-size:0.95rem;
   line-height: 1.7;
 }

 a {
  display: inline-block;
  font-size: 0.85rem;
  padding: 10px 30px;
  text-transform: uppercase;
  text-decoration: none;
  font-weight: 500;
  margin-top: 30px;
  background-color: #262626;
  color: #fff;
  border-radius: 20px;
  letter-spacing: 2px;
  transition: 0.3s;
}
a:hover {
  background-color: #dc3d04
}


 .row-reverse {
    width: 100%;
    max-width: 1200px;
    margin: 0px auto;
    padding: 0rem 1.2rem;
    display: flex;
    align-items: center;
    flex-direction: row-reverse;
 }

 .row-reverse .right-row {
   margin-right: -100px;
 }

 .left-row2 {
   background: url("@/assets/Agrosample.jpg");
   width: 50%;
   height: 500px;
    background-size: cover;
    background-repeat: no-repeat;
    background-position: center;
 }


 .left-row3 {
    background: url("@/assets/field2.jpg");
    background-size: cover;
    background-repeat: no-repeat;
    background-position: center;
    width: 50%;
    height: 450px;
 }

@media only screen and (max-width: 1024px) {
  .row, .row-reverse {
    flex-direction: column;
  }

  .right-row {
    margin-left: 0;
    margin-right: 0;
    margin-top: -100px;
    width: 95%;
  }

  #about-rows > div.row-reverse > div.right-row {
    margin-left: 0;
    margin-right: 0;
  }

  .image {
    height: 60vw;
    width: 100%;
  }

}

  @media only screen and (max-width: 576px) {
    .right-row {
      width: 95%;
    }

    p{
      line-height: 1.6;
      font-size: 0.9rem;
    }

    h3 {
      font-size: 1.5rem;
    }

    h5 {
      font-size: 1rem;
    }

    .image {
    height: 100vw;
    width: 100%;
  }

  .right-row {
    padding: 35px 30px;
    margin-top: -70px;
  }


  }
  
</style>