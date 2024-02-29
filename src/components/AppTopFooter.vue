<script>

export default{
    name:"AppTopFooter",
  
  data(){
    
    return{
        elements:[

        {
         title:'DC COMICS',
         list:["Characters","Comics","Movies","TV","Games","Videos","News"]
        },

        {
        title:'SHOP',
         list:["Shop DC","Shop DC Collectibles"]
        },

        {
         title:'DC',
         list:["Terms Of Use","Privacy policy(New)","Ad Choices","Advertising","Jobs","Subscriptions","Talent Workshops","CPSC Certificates","Ratings","Shop Help","Contact Us"]
        },

        {
        title:'SITES',
         list:["DC","MAD Magazine","DC Kids","DC Universe","DC Power Visa"]
        }



        ]

        

    }
  }

}
</script>

<template>
    <div id="top-footer">
        <div class="container4">
        <ul>
            <li v-for="element in elements" class="list-title">
                {{ element.title }}
                <li v-for="listElement in element.list" class="list">{{ listElement }}</li>
            </li>
            

        </ul>

        <img src="/img/dc-logo-bg.png" alt="">
       </div>
     </div>

</template>

<style>
.container4{
  max-width: 1200px;
  height: 370px;
  margin-left: auto;
  margin-right: auto;
  display: flex;
  justify-content: space-between;
}

 #top-footer{
    border: 1px white solid;
    background-image: url("/img/footer-bg.jpg");
     background-position: center;
     background-size: cover;
 }

 .list{
    color: gray;
 }

 
</style>