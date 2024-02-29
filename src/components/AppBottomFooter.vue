<script>

export default{
    name:"AppBottomFooter",
  
  data(){
    
    return{

    }
  }

}
</script>

<template>
    <div id="bottom-footer">
        <div class="container5">

       <button>SIGN-UP NOW!</button>

        <div class="socials">
            <span>FOLLOW US</span>
            <img src="/img/footer-facebook.png" alt="">
            <img src="/img/footer-twitter.png" alt="">
            <img src="/img/footer-youtube.png" alt="">
            <img src="/img/footer-pinterest.png" alt="">
            <img src="/img/footer-periscope.png" alt="">
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
  padding: 30px;
  display: flex;
  justify-content: space-between;
}

 /*#bottom-footer{
    border: 1px white solid;
 }*/

 button{
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