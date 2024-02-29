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
    <div class="container">  
<img src="/img/dc-logo.png" alt="dc_logo">

<ul>
    <li v-for="link in links">{{link}}</li>
</ul>

  </div>
    </header>

</template>

<style>

.container{
  max-width: 1200px;
  margin-left: auto;
  margin-right: auto;
  display: flex;
align-items:center;
justify-content: space-between;
}

 header{
    border: 1px white solid;
 }

 ul{
    list-style-type: none;
    display: flex;
    gap: 20px;
 }
</style>