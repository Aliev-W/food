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
