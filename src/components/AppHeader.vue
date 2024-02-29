<script>

export default{
    name:"AppHeader",
  
  data(){
    
    return{
     links:["CHARACTERS","COMICS","MOVIES","TV","GAMES","COLLECTIBLES","VIDEOS","FANS","NEWS","SHOP"]

    }
  }

}
</script>

<template>
    
    <header> 
  <div class="container1">
<img src="/img/dc-logo.png" alt="dc_logo">

<ul>
    <li v-for="link in links" class="link">{{link}}</li>
</ul>
  </div>
    </header>

</template>

<style lang="scss">
$primaryColor:rgba(2, 130, 249, 1);

.container1{
  max-width: 1200px;
  margin-left: auto;
  margin-right: auto;
  padding: 20px 0;
  display: flex;
align-items:center;
justify-content: space-between;
}

 header{
    border: 1px white solid;
    background-color: white;
    color: black;
 }

 ul{
    list-style-type: none;
    display: flex;
    gap: 30px;

    .link{
    font-weight: bolder;
   }
   
 
 .link:active{
     color:$primaryColor;
    }
 }

 
</style>