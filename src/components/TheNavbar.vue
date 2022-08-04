<template>
   <header>
        
        <ul class="navigation">
            <li><a href="#" class="logo"><img src="../assets/logo.png" alt=""></a></li>
            <li><a href="#home">Home</a></li>
            <li><a href="#about">About us</a></li>
            <li><a href="#menu">Menu</a></li>
            <li><a href="#features">Features</a></li>
            <li><a href="#contact">Contact us</a></li>
        </ul>
        <a href="#"><button class="btn">Booking Now</button></a>
    </header>

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
</template>

<script>
export default {
   name: 'TheNavbar'
}
</script>

<style lang="scss" scoped>
@import url(https://fonts.googleapis.com/css?family=Roboto:400,500);
@import url(https://fonts.googleapis.com/css?family=Philosopher:700);

*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Poppins', sans-serif;
    scroll-behavior: smooth;
}

header{
    top: 0;
    left: 0;
    width: 100%;
    padding: 40px 100px;
    z-index: 10000;
    display: flex;
    justify-content: space-between;
    align-items: center;
    transform: 0.5s;
}

header .navigation{
    display: flex;
    justify-content:flex-start;
    align-items: center;
}

header .navigation li{
    list-style: none;
    margin-left: 40px;
    font-family: Roboto;
}

header .navigation li a img{
   width: 45px;
   height: 45px;
}

header .navigation li a{
    text-decoration: none;
    color: #150C01;
    font-size: 16px;
    font-weight: 500;
    opacity: 0.6;
}

header .navigation li a:hover{
    color: #DC780B;
}

header .btn{
   position: absolyut;
   width: 155px;
   height: 46px;
   background: #DC780B;
   border-radius: 5px;
   border: 0;
   cursor: pointer;
   margin-right: 50px;

   font-family: Roboto;
   font-weight: 400;
   font-size: 16px;
   line-height: 19px;
   color: #fff;
}

.food{
   display: flex;
   justify-content: space-between;
}

section .text{
   width: 555px;
   margin-left: 150px;
}

.food .title{
   font-family: Philosopher;
   font-weight: 700;
   font-size: 50px;
   line-height: 58px;
   margin-top: 175px;
    color: #150C01;
}

.food .sub{
   font-family: Roboto;
   font-weight: 500;
   font-size: 16px;
   line-height: 24px;
   margin-top: 40px;
   color: #150C01;
   opacity: 0.7;
}

.food .btns{
   margin-top: 50px;
}

.btns button{
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
   
}

.btns button:hover{
   background: #DC780B;
   color: #fff;
}

.btns button:nth-child(1){
   margin-right: 30px;
}
section .parent{
   width: 801px;
   height:670px;
   margin-top: -40px;
}
section .parent .child{
   width: 100%;
   height: 100%;
   background: url(../assets/food.png);
   background-repeat: no-repeat;
   background-position: center;
   background-size: cover;
   margin-right: 1050px;
}

.Features{
   text-align: center;
}

.Features p{
   font-family: Roboto;
   font-weight: 500;
   font-size: 16px;
   line-height: 19px;
   letter-spacing: 0.2em;
   color: #DC780B;
   opacity: 0.7;
   margin-top: 100px;
}
.Features h3{
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
   margin-top: 45px;
   gap: 150px;
}

.cards .card{
   width: 300px;
   text-align: center;
}

.cards .card .block{
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

.cards .card img{
   margin-top: 20px;
}

.cards .card h4{
   margin-top: 50px;
   font-family: Philosopher;
   font-weight: 700;
   font-size: 25px;
   line-height: 24px;
   color: #150C01;
}

.cards .card h5{
   font-family: Roboto;
   font-weight: 400;
   font-size: 16px;
   line-height: 24px;
   text-align: center;
   color: #150C01;
   opacity: 0.7;
   margin-top: 15px;
}

.about{
   display: flex;
   justify-content: center;
   margin-top: 100px;
}

.about img{
   border-radius: 35px;
}

.about .us{
   margin-left: 130px;
   margin-top: 100px;
}

.about .us h4{
   
   font-family: Roboto;
   font-weight: 500;
   font-size: 16px;
   line-height: 24px;
   display: flex;
   align-items: center;
   letter-spacing: 0.2em;
   text-transform: uppercase;
   color: #DC780B;
   opacity: 0.7;
}

.about .us h3{
   width: 500px;
   font-family: 'Philosopher';
   font-weight: 700;
   font-size: 32px;
   line-height: 41px;
   color: #150C01;
   margin-top: 10px;
}

.about .us p{
   width: 500px;
   margin-top: 30px;
   font-family: Roboto;
   font-weight: 400;
   font-size: 16px;
   line-height: 24px;
   color: #150C01;
   opacity: 0.7;
}

.about .us button{
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
}
</style>
