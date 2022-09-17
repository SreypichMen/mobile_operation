
<template>
    <nav v-scroll="handleScroll" >
    <div id="box1" class="box">
     <header >
            <div class="nav1 flex-none mt-1 ">
              <nuxt-link to="/">
                <img src="~/assets/img/moc logo.png" alt="">
              </nuxt-link>
            </div>
    
      <div class="nav2  ">
              <ul>
                <li style="text-decoration: none"> <h2>Home</h2></li>
                <li  style="text-decoration: none"> <h2>Cellcard</h2></li>
                <li  style="text-decoration: none"> <h2>Smart</h2></li>
                <li  style="text-decoration: none"> <h2>Metfone</h2></li>
                <li  style="text-decoration: none"> <h2>Seatel</h2></li>
              
              </ul>
             
   </div>
        </header>
        </div>
        </nav>
    </template>
    
    <script>
      export default {
        data () {
          return {
          
            
          }
        },
         methods: {
          handleScroll: function (evt, el) {
            var box1 = document.getElementById('box1')
              if (window.scrollY <80) {
                  box1.classList.remove('box1');
          }
          else {
            box1.classList.add('box1');
          }
        
        }
    
      
      }}
    </script>
    
    <style scoped>
    
    
    .box{
     
      font-size: medium;
      position: fixed;
      /* position: sticky; */
      top:0;
      scroll-behavior: smooth;
      z-index: 10000;
      width:100%;
      transition: all 1s;
      /* background-color: whitesmoke; */
      background-color:transparent;
      /* backdrop-filter: blur(2px); */
     border-bottom: 2px solid #0001;
     color: white;
    }
    .box1{
      background-color: whitesmoke;
      border-bottom: 2px solid whitesmoke;
         color: #ED213A;
    }
  
    
    .nav1{
        height: 60px;
        width: 30%;
        float:left;
        margin-left:40px;
    }
    .nav_bar{
          margin-top: 14px;
          padding: 10px;
    }
    
    
    li--active {

      color: black!important;
      
      
      transition:0.1s all;
     
      font-weight: bold;
     
    }
    
    .h2:hover{
    
      
      color: #6f0000!important;
    

      transition:0.1s all;
      font-weight: bold;
      color: white!important;
    
    }
    .nav1{
        height: 50px;
        width: 30%;
        float:left;
       
      
    }
    .icon{
        color:black!important;
      margin-bottom: 2px;
      margin-right: 5px;
    }
    
   
    h4{
        font-weight: bold;
        font-size: 1rem;  
    }
    p{
         
      font-size: 0.8rem;
    }
    
    .pic{
     
        height: 400px;
        width: 100%;
        padding-top: 20px;
        padding-left:20px;
        padding-bottom:20px;
    }
   
    h2{
        /* color: black; */
      
        font-size:1rem;
        
    }
    h5{
        font-size: 0.8rem;
    }
    ul{
        padding: 20px;
        display:flex;
       
        gap: 50px;
        list-style-type: none;
    }
    li:hover{
        color: black;
    }
   
    
    @media screen and (max-width: 992px) {
        img{
         height: 55px;
         width: 20%;
    }
    }
    @media screen and (max-width:572px){
       img{
         margin-top: 10px;
         height: 30px;
         width: 40%;
    }
    }
    @media screen and (min-width: 992px) {
        img{
        height:55px;
        width: 20%;
    }}
    
    @media screen and (max-width: 1010px) {
    
      .nav2{
      
        display:none;
    }
    
    }
    
    @media screen and (min-width: 1010px) {
       .nav2{
      
        height: 60px;
        width: 50%;
        float:right;
        display: flex;
        justify-content:flex-end;
        gap: 5px;
        margin-right:40px;
    }
    img{
        height:55px;
        width: 15%;
    }
     
    }
    
    
    
    
    
    </style>
    
    
    
    
    