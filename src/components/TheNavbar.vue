<template>
   <header :class="{'scrolled-nav':scrolledNav}">
        <nav>
         <div class="branding">
            <img src="../assets/logo.png" alt="">
         </div>
         <ul v-show="!mobile" class="navigation">
            <li><router-link class="link" :to="{name: 'home'}">Home</router-link></li>
            <li><router-link class="link" :to="{name: 'about'}">About</router-link></li>
            <li><router-link class="link" :to="{name: 'menu'}">Menu</router-link></li>
            <li><router-link class="link" :to="{name: 'features'}">Features</router-link></li>
            <li><router-link class="link" :to="{name: 'contact'}">Contact</router-link></li>
            
        </ul>

        <div class="icon">
         <i @click="toggleMobileNav" v-show="mobile" class="far fa-bars" :class="{'icon-active':MobileNav}"></i>
        </div>

        <transition name="mobile-nav">
         <ul v-show="mobileNav" class="dropdown-nav">
            <li><router-link class="link active" :to="{name: 'home'}">Home</router-link></li>
            <li><router-link class="link" :to="{name: 'about'}">About</router-link></li>
            <li><router-link class="link" :to="{name: 'menu'}">Menu</router-link></li>
            <li><router-link class="link" :to="{name: 'features'}">Features</router-link></li>
            <li><router-link class="link" :to="{name: 'contact'}">Contact</router-link></li>
            
        </ul>
        </transition>
        </nav>
        <a href="#"><button class="btn">Booking Now</button></a>
    </header>
</template>

<script>
export default {
   name: "TheNavbar",
   data(){
      return{
         scrolledNav:null,
         mobile:null,
         mobileNav:null,
         windowWidth:null,
   };
},

created(){
   window.addEventListener("resize", this.checkScreen);
   this.checkScreen();
},

mounted() {
   window.addEventListener("scroll", this.updateScroll);
},

methods:{
   toggleMobileNav(){
      this.mobileNav = !this.mobileNav
   },

   updateScroll(){
      const scrollPosition = window.scrollY;
      if(scrollPosition > 50){
         this.scrolledNav = true;
         return;
      }
      this.scrolledNav=false;
   },

   checkScreen(){
      this.windowWidth = window.innerWidth;
      if(this.windowWidth <= 750){
         this.mobile = true;
         return;
      }
      this.mobile = false;
      this.mobileNav =false;
      return;
   },
},
};
</script>

<style lang="scss" scoped>

header{
   background-color: #fff;
   z-index: 99;
   width: 100%;
   position: fixed;
   transition: .5s ease all;
   color: #150C01;
   display: flex;

   nav{
   position: relative;
   display: flex;
   flex-direction: row;
   padding: 31px 0;
   padding-bottom: 0;
   transition: .5s ease all;
   width: 90%;
   // margin: 0 150px;
   @media(min-width: 1140px){
      max-width: 1140px;
   }

   ul,
   .link{
      display: flex;
      font-weight: 500;
      font-family: Roboto;
      color: #150C01;
      list-style: none;
      text-decoration: none;
   
   }
   
   li{
      padding-top: 5px;
      padding-right: 40px;
      transform: 0.5s ease all;
      border-bottom: 1px solid transparent;
      opacity: 0.6;
      a{&:hover{
         color: #DC780B;
      }}
      
   }
   .branding{
      display: flex;
      align-items: center;
      margin-left: 150px;

      @media (max-width: 750px) {
         margin-left: 100px;
      }

      img{
         width: 44px;
         transform: .5s ease all;
      }
   }

   .navigation{
      display: flex;
      align-items: center;
      flex: 1;
      justify-content: flex-start;
      margin-left: 40px;

      @media(max-width: 1315px){
      text-align: center;
      justify-content: center;
   }
   }

   .icon{
      display: flex;
      align-items: center;
      position: absolute;
      top: 0;
      right: 24px;
      height: 100%;
      color: #150C01;
      padding-top: 30px;
      i{
         cursor: pointer;
         font-size: 24px;
         transition: 1s ease all;
      }
   }

   .icon-active{
      transform: rotate(180deg);
   }

   .dropdown-nav{
      display: flex;
      flex-direction: column;
      position: fixed;
      width: 50%;
      height: 100%;
      min-width: 250px;
      background-color: #fff;
      
      li{
         margin: 10px;

         &:hover{
            color: #DC780B;
            font-weight: 700;
            font-family: Roboto;
         }
      }
   }

   .mobile-nav-enter-active,
   .mobile-nav-leave-active{
      transition: 1s ease all;
   }

   .mobile-nav-enter-from,
   .mobile-nav-leave-to{
      transform: translateX(-250px);
   }

   .mobile-nav-enter-to{
      transform: translateX(0);
   }
}
}

.btn{
      position: absolyut;
   width: 155px;
   height: 46px;
   background: #DC780B;
   border-radius: 5px;
   border: 0;
   cursor: pointer;
   margin-top: 30px;
   margin-left: 460px;
   
   font-family: Roboto;
   font-weight: 400;
   font-size: 16px;
   line-height: 19px;
   color: #fff;

    @media(max-width: 1315px){
      display: none;
   }
   }

.scrolled-nav{
   background-color: #fff;
   box-shadow: 0 4px 6px -1px rgba(255, 255, 255, 0.8), 0 2px 4px -1px rgba(255, 255, 255, 0.7);

   nav{
      padding: 8px 0;

      .branding{
         img{
            width: 40px;
            box-shadow: 0 4px 6px -1px rgba(255, 255, 255, 0.8), 0 2px 4px -1px rgba(255, 255, 255, 0.7);
         }
      }
      li{
         color: #fff;
      }
   }
}
</style>