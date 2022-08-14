<template>
   <section class="food" id="home">
      <div class="text">
         <div class="title">Making time a good time by making food the good food.</div>
         <div class="sub">There are many things are needed to start the Fast Food Business. You need not only Just Food Stalls with Persons but also specialized equipment,</div>
         <div class="btns">
            <button >Order Now</button>
            <button >Food Details</button>
         </div>
      </div>
      <div class="parent">
         <div class="child"></div>
      </div>
   </section>

   <div class="about" id="about">
         <img src="../assets/about.png" alt="">
         <div class="us">
            <h4>About us</h4>
            <h3>Food Stalls with Persons but  to  Product marketing plane
catlogues etc to. </h3>
            <p>There are many things are needed to start the Fast Food Business. You need not only Just Food Stalls with Persons but also 
equipment  make your marketing plane Effective.</p>
            <button>Read More</button>
            </div>
   </div> 

   <div class="Features" id="features">
      <p>FEATURES</p>
      <h3>Food with a New Passion</h3>

      <div class="cards">
         <div class="card card1">
            <div class="block"></div><img src="../assets/features1.png" alt="">
            <h4>Quality Food</h4>
            <h5>It can be a very secure path to earn good money and make you very successful creative entrepreneur.</h5>
         </div>

         <div class="card card2">
            <div class="block"></div><img src="../assets/features2.png" alt="">
            <h4>Food Delivery</h4>
            <h5>It can be a very secure path to earn good money and make you very successful creative entrepreneur.</h5>
         </div>

         <div class="card card3">
            <div class="block"></div><img src="../assets/features3.png" alt="">
            <h4>Super Taste</h4>
            <h5>It can be a very secure path to earn good money and make you very successful creative entrepreneur.</h5>
         </div>
      </div>
   </div>
</template>

<script>
export default {
  name: 'HomeView'
}
</script>

<style lang="scss" scoped>
.food{
   display: flex;
   justify-content: space-between;
   height: 700px;

   @media (max-width:750px) {
      height: 350px;
   }

   .text{
   width: 555px;
   margin-left: 150px;

   @media (max-width: 1000px) {
      margin: 0 auto;
      
   }

   .title{
   font-family: Philosopher;
   font-weight: 700;
   font-size: 50px;
   line-height: 58px;
   margin-top: 235px;
    color: #150C01;

    @media (max-width:750px) {
      margin: 120px auto;
      margin-bottom: 20px;
      font-size: 30px;
      line-height: 30px;
      text-align: center;
      }
}

.sub{
   font-family: Roboto;
   font-weight: 500;
   font-size: 16px;
   line-height: 24px;
   margin-top: 40px;
   color: #150C01;
   opacity: 0.7;

   @media (max-width:750px) {
      font-size: 16px;
      line-height: 20px;
      text-align: center;
      }
}

.btns{
   margin-top: 50px;

   @media (max-width:750px) {
      text-align: center;
      }

   button{
   width: 158px;
   height: 60px;
   cursor: pointer;
   background: #fffefe;
   box-sizing: border-box;
   border: 1.5px solid #e9dac9;
   border-radius: 5px;

   
   font-family: Roboto;
   font-weight: 500;
   font-size: 16px;
   line-height: 19px;
   color: #DC780B;

   @media (max-width:750px) {
      width: 120px;
      height: 40px;
      font-size: 15px;
      font-weight: 500;
      }
   
   &:hover{
      background: #DC780B;
   color: #fff;
   }
}
}
}

.parent{
   width: 801px;
   height:670px;
   margin-top: 40px;

   @media (max-width: 1000px) {
      display: none;
   }

   .child{
   width: 100%;
   height: 100%;
   background: url(../assets/food.png);
   background-repeat: no-repeat;
   background-position: center;
   background-size: cover;
   margin-right: 1050px;
}
}
.btns button:nth-child(1){
   margin-right: 30px;
}
}

.about{
   display: flex;
   justify-content: space-between;

   @media (max-width:750px) {
      display: grid;
      justify-content: space-around;
      }

   img{
   border-radius: 35px;
   margin-left: 200px;

   @media(max-width: 1440px){
      width: 300px;
      height: 280px;

      @media (max-width:750px) {
         width: 150px;
         height: 140px;
         align-items: center;
         margin: 120px auto;
         margin-bottom: 0;
      }
   }
}

.us{
   margin-right: 200px;


   @media (max-width:750px) {
      margin: 20px auto;
      text-align: center;
      }

   h4{
   
   font-family: Roboto;
   font-weight: 500;
   font-size: 16px;
   line-height: 24px;
   display: flex;
   letter-spacing: 0.2em;
   text-transform: uppercase;
   color: #DC780B;
   opacity: 0.7;

   @media (max-width:750px) {
      margin: 0 auto;
      justify-content: center;
      }
}

h3{
   width: 500px;
   font-family: 'Philosopher';
   font-weight: 700;
   font-size: 32px;
   line-height: 41px;
   color: #150C01;
   margin-top: 10px;

   @media (max-width:750px) {
      font-size: 22px;
      line-height:30px;
      }
}

p{
   width: 500px;
   margin-top: 30px;
   font-family: Roboto;
   font-weight: 400;
   font-size: 16px;
   line-height: 24px;
   color: #150C01;
   opacity: 0.7;

   @media (max-width:750px) {
      margin-top: 20px;
      font-size: 16px;
      }
}

button{
   width: 142px;
   height: 42px;
   background: #DC780B;
   border-radius: 5px;
   border: none;
   margin-top: 30px;
   cursor: pointer;

   color: #fff;
   font-family: Roboto;
   font-weight: 500;
   font-size: 16px;
   line-height: 19px;

   @media (max-width:750px) {
      width: 120px;
      height: 30px;
      font-size: 15px;
      font-weight: 400;
      }
}
}
}

.Features{
   text-align: center;
   margin-top: 80px;

   p{
   font-family: Roboto;
   font-weight: 500;
   font-size: 16px;
   line-height: 19px;
   letter-spacing: 0.2em;
   color: #DC780B;
   opacity: 0.7;
}

h3{
   font-family: Philosopher;
   font-weight: 700;
   font-size: 32px;
   line-height: 35px;
   text-transform: capitalize;
   color: #150C01;
   margin-top: 10px;
}

.cards{
   display: flex;
   justify-content: center;
   margin-top: 70px;
   gap: 150px;

   @media (max-width:1200px) {
      display: grid;
      gap: 20px;
   }

   .card{
   width: 300px;
   text-align: center;

   .block{
   position: absolute;
   display: flex;
   justify-content: center;
   z-index: 11;
   width: 88px;
   height: 88px;
   background: #E64D2E;
   opacity: 0.08;
   border-radius: 50%;
   margin-left: 105px;
}

h4{
   margin-top: 50px;
   font-family: Philosopher;
   font-weight: 700;
   font-size: 25px;
   line-height: 24px;
   color: #150C01;
}

img{
   margin-top: 20px;
}

h5{
   font-family: Roboto;
   font-weight: 400;
   font-size: 16px;
   line-height: 24px;
   text-align: center;
   color: #150C01;
   opacity: 0.7;
   margin-top: 15px;
}
}
}
}






</style>
