<template>
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
  name: 'AboutView'
}
</script>

<style lang="scss" scoped>
.about{
   display: flex;
   justify-content: space-between;
   margin: auto;

   @media (max-width:750px) {
      justify-content: space-around;
      }

   img{
   margin-top: 150px;
   border-radius: 35px;
   margin-left: 200px;

   @media(max-width: 1315px){
      width: 300px;
      height: 300px;

      @media (max-width:750px) {
         width: 150px;
         height: 150px;
      }
   }
}

.us{
   margin-right: 200px;
   margin-top: 150px;

   h4{
   
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

   @media (max-width:750px) {
      margin: 0 auto;
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
      font-size: 20px;
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
}
}

}
</style>
