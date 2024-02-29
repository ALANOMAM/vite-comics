<script>

export default{
    name:"AppBodyNav",
  
  data(){
    
    return{

    }
  }

}
</script>

<template>
    <div id="body-nav">
    <div class="container3">
     <div class="icon">
        <img src="/img/buy-comics-digital-comics.png" alt="">
        <span>DIGITAL COMICS</span>
    </div>

     <div class="icon">
        <img src="/img/buy-comics-merchandise.png" alt="">
        <span>DC MERCHANDISE</span>
    </div>

     <div class="icon">
        <img src="/img/buy-comics-subscriptions.png" alt="">
        <span>SUBSCRIPTION</span>
    </div>

     <div class="icon">
        <img src="/img/buy-comics-shop-locator.png" alt="">
        <span>COMIC SHOP LOCATOR</span>
    </div>

     <div class="icon">
        <img src="/img/buy-dc-power-visa.svg" class="visa" alt="">
        <span>DC POWER VISA</span>
    </div>
    </div>
     </div>

</template>

<style lang="scss">
$primaryColor:rgba(2, 130, 249, 1);

.container3{
  max-width: 1200px;
  margin-left: auto;
  margin-right: auto;
  padding: 50px 0;
  display: flex;
  align-items: center;
  justify-content: space-between;

  img{
      width: 60px;
      height: auto;
  }
}

.icon{
    display: flex;
    align-items: center;
    gap:20px;
}
 #body-nav{
   /* border: 1px white solid;*/
    background-color: $primaryColor;
 }


</style>