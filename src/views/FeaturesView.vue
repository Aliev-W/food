<template>
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
  name: 'FeaturesView'
}
</script>

<style lang="scss" scoped>

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
</style>
