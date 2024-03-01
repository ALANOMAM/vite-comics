<script>

export default{
    name:"AppBottomFooter",

  
  data(){
    
    return{
        socialMedia:[
        "/img/footer-facebook.png",
        "/img/footer-twitter.png",
        "/img/footer-youtube.png",
        "/img/footer-pinterest.png",
        "/img/footer-periscope.png"
        ]
    }
  }

}
</script>

<template>
    <div id="bottom-footer">
        <div class="container5">

       <button class="btn">SIGN-UP NOW!</button>

        <div class="socials">
            <span>FOLLOW US</span>
            <div v-for="social in socialMedia">
                <img :src="social" alt="">
            </div>
        </div>

        </div>
  
     </div>

</template>

<style lang="scss">
$primaryColor:rgba(2, 130, 249, 1);

.container5{
  max-width: 1200px;
  margin-left: auto;
  margin-right: auto;
  padding: 30px 0;
  display: flex;
  justify-content: space-between;
}

 /*#bottom-footer{
    border: 1px white solid;
 }*/

 .btn{
    padding: 10px;
    font-size: 20px;
    border: 2px solid $primaryColor;
    background-color: rgba(48, 48, 48, 1);
    color: white;
 }

 .socials{
    display: flex;
    gap:20px;
    align-items: center;
    span{
        color:$primaryColor;
        font-weight: bolder;
        font-size: 25px;
    }
 }
</style>