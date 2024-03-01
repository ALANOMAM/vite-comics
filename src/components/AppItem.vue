<script>
export default{
      name:"AppItem",

      props:{
        comName: String,
        comImage: String
      },

    data(){
        return{

        }
    }
}
</script>

<template>

<div class="dcItem">
        <img  :src="comImage" alt="">
        <span>{{ comName }}</span>
</div>

</template>

<style lang="scss">
.dcItem{
  width: calc(100% / 6);  
  padding: 20px;
  display: flex;
  flex-direction: column;
  gap:10px;

    img{
        width:100%;
        height:200px;
    }
}

</style>