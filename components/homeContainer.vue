<template>
    <div class="wrapper">
    <div class="poster ">
        <swiper class="swiper" :options="swiperOption">
          <swiper-slide >
            <v-img  class="size" src="https://www.cellcard.com.kh/c/uploads/2022/07/TimeToRise_Vannda_Mobile_Site_720x460-1.jpeg">
            </v-img>
          </swiper-slide>
          <swiper-slide >
            <v-img  class="size" src="https://www.smart.com.kh/media/2022/06/Chey-Kroy_Home-page_Desktop_KH.png">
            </v-img>
          </swiper-slide>
          <swiper-slide >
            <v-img  class="size" src="https://metfone.com.kh/Uploads/files/49079364_2014241061997993_2101896753451106304_n.png">
         
            </v-img>
          </swiper-slide>
          <swiper-slide >
            <v-img  class="size" src="https://api.yes.com.kh/uploads/1608857296863-1080-x-900.jpg">
          
            </v-img>
          </swiper-slide>
       
        <div class="swiper-button-prev" slot="button-prev"></div>
        <div class="swiper-button-next" slot="button-next"></div>
        <div class="swiper-pagination" slot="pagination"></div>
      </swiper>
    
        </div>
      <div style="margin-top:5%">
        <HomeDetails />
      </div>
    
    
    </div>
    
    </template>
    <script>
    import homeDetails from '~/components/homeDetails.vue';
    import { Swiper, SwiperSlide } from 'vue-awesome-swiper'
      import 'swiper/css/swiper.css'
    
      export default {
        name: 'swiper-example-navigation',
        title: 'Navigation',
        components: {
          Swiper,
          SwiperSlide,
          homeDetails
         
        },
        data() {
          return {
            swiperOption: {
                effect: 'fade',
              autoplay:{
                delay: 30000,
                displayOnInteraction: false
              },
              navigation: {
                nextEl: '.swiper-button-next',
                prevEl: '.swiper-button-prev'
              }, 
              pagination: {
                el: '.swiper-pagination'
              }
            }
          }
        } ,methods: {
      goTo(id) {
  
         this.$router.push('/newsblog/' + id)
      }
    }
      }
     
    
    
      
    </script>
    <style scoped>
    .pd{
        padding-left: 60px;
        padding-right: 50px;
        
    }
    @media screen and (max-width: 992px) {
       
     .poster{
      
    
        width:100%;
        height: 500px ;
     
    }
       .size{
      
      height: 500px;
      width: 100%;
        
    
    
      }
    }
    @media screen and (max-width: 572px) {
    .poster{
      
    
        width:100%;
        height: 300px ;
     
    }
       .size{
      
      height: 300px;
      width: 100%;
      }
      h1{
    font-size:1.3rem;
    margin-bottom: 300px;
  
  }
  h2{
    
    font-size: 15px;
  }
  h3{
    
    font-size: 13px;
  }
  @keyframes typewriter{
       to{
        left: 100%;
      }  
      0%{
        width: 0;
      }
      50%{
        width:350px;
      }
    }
    }
    
  
  
  
  @media screen and (min-width: 992px) {
       .poster{
        width:100%;
        height: 650px ;
      }
      .size{
      
      height: 650px;
      width: 100%;
    
      }
      h1{
      color:whitesmoke;
       font-size: 1.7em;
      width: max-content;
      overflow: hidden;
      white-space:nowrap;
      animation: typewriter 4s steps(28) forwards infinite;
      border-right: 3px solid orange;
    }
    h3{
        font-size: 2em;
        overflow: hidden;
      white-space:nowrap;
    }
    @keyframes typewriter{
       to{
        left: 100%;
      }  
      0%{
        width: 0;
      }
      50%{
        width:480px;
      }
    }
  .img{
    height: 700px;
    width: 100%;
  }
    }
    
    </style>
    
   
    
    