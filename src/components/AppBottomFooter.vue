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

 #bottom-footer{
    border: 1px white solid;
 }

 button{
    padding: 10px;
    border: 2px solid $primaryColor;
    background-color: rgba(48, 48, 48, 1);
    color: white;
 }

 .socials{
    span{
        color:$primaryColor;
        font-weight: bolder;
        font-size: 25px;
    }
 }
</style>