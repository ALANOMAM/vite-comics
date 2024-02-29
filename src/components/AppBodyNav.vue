<script>

export default{
    name:"AppBodyNav",
  
  data(){
    
    return{

        options:[
            { title:"DIGITAL COMICS",
              image:"/img/buy-comics-digital-comics.png"
            },

            {
             title:"DC MERCHANDISE",
              image:"/img/buy-comics-merchandise.png"
            },

            {
              title:"SUBSCRIPTION",
              image:"/img/buy-comics-subscriptions.png"
            },

            {
             title:"COMIC SHOP LOCATOR",
             image:"/img/buy-comics-shop-locator.png"
            },

            {
             title:"DC POWER VISA",
              image:"/img/buy-dc-power-visa.svg"
            }

        ]

    }
  }

}
</script>

<template>
    <div id="body-nav">
    <div class="container3">

        <div v-for="option in options" class="icon">
        <img :src="option.image" alt="">
        <span>{{ option.title }}</span>
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