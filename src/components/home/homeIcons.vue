<template>
   <section id="icons">
     <div id="icons-container">
        <div class="investment-text">
          <h2>Tripple bottom line</h2>
          <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit.</p>
        </div>
          <div class="icons-wrapper">
              <div class="right icon "><i class="fa-solid fa-people-arrows-left-right"></i>
            <h5>Social equity </h5>
            <p>Odio aliquet, fringilla odio eget, tincidunt nunc duis aliquet pulvinar employees and organizations.</p>
          </div>
            <div class="left icon"><i class="fa-solid fa-chart-line"></i>
            <h5>Economic </h5>
            <p>Odio aliquet, fringilla odio eget, tincidunt nunc duis aliquet pulvinar employees and organizations.</p>
            </div>
          
          
            <div class="center icon "><i class="fa-solid fa-earth-europe"></i>
            <h5>Environmental </h5>
            <p>Odio aliquet, fringilla odio eget, tincidunt nunc duis aliquet pulvinar employees and organizations.</p>
            </div>
          <div class="filler icon">
           
          </div>
          </div>
        </div>
    </section>
</template>

<style scoped>

#icons {
  background: #fff;
  position: relative;
}

#icons-container {
  width: 100%;
  max-width: 1200px;
  line-height: 1.4;
  margin: 0px auto;
  padding: 120px 1.2rem;
}

.icons-wrapper  i {
  background-color: #59b555;
  font-size: 2rem;
  padding: 2rem;
  border-radius: 50%;
  margin-bottom: 35px;
  color: #fff;
  transition: 0.2s;

}


.investment-text {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  margin-bottom: 90px;
  text-align: center;
}



.investment-text h2 {
  font-family: 'Lora', serif;
  font-size: 2.5rem;
  margin-bottom: 1.5rem;
}

.investment-text p {
  color: #6a6063;
}

.icons-wrapper {
  display: flex;
  justify-content: center;
  align-items: center;

}

.icons-wrapper h5 {
  font-size: 1.5rem;
  font-family: 'Lora', serif;
  margin-bottom: 20px;
  color: #59b555;
}

.icons-wrapper p {
  font-weight: 300;
  margin: 5px 0px 30px 0px;
  color: #6a6063;
}


.icons-wrapper div {
  display: flex;
  flex-direction: column;
  justify-content: center;  
  align-items: center;
  text-align: center;
}

.left, .center, .right {
  padding: 0rem 3rem;
}


@media only screen and (max-width: 1024px) {
  .icons-wrapper  {
    flex-flow: wrap;
    gap: 20px;
  }

  .icon{
    flex-basis: 40%;
  }

  .center {
    padding: 1.5rem 1.5rem 0rem 1.5rem;
  }

  .left, .center, .right {
    padding: 1.5rem;
  }


}

  @media only screen and (max-width: 767px) {
    .icons-wrapper h5 {
      font-size: 1.4rem;
    }

    .icons-wrapper p {
      font-size: 0.95rem;
    }

    .investment-text h2 {
      font-size: 2.2rem;
    }
    
    
   .investment-text p {
    font-size: 0.95rem;
   }
    
  }


  @media only screen and (max-width: 576px)
   {
     .icons-wrapper {
      flex-direction: column;
      flex-wrap: nowrap;
     }

      .investment-text h2 {
        font-size: 1.85rem;
    }

    .investment-text {
      margin-bottom: 50px;
    }

     .center {
    padding: 1.5rem 1.5rem 0rem 1.5rem;
  }

  #icons-container {
    padding: 100px 1.2rem;
  }

   }
</style>
