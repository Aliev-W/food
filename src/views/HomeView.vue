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
   height: 100vh;
}

section .text{
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
}

.sub{
   font-family: Roboto;
   font-weight: 500;
   font-size: 16px;
   line-height: 24px;
   margin-top: 40px;
   color: #150C01;
   opacity: 0.7;
}

.btns{
   margin-top: 50px;

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
   
   &:hover{
      background: #DC780B;
   color: #fff;
   }
}
}
}

.btns button:nth-child(1){
   margin-right: 30px;
}
section .parent{
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

</style>
