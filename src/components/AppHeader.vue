<script>

export default{
    name:"AppHeader",
  
  data(){
      
    return{
     activeLinkIndex:0,

     links:["CHARACTERS","COMICS","MOVIES","TV","GAMES","COLLECTIBLES","VIDEOS","FANS","NEWS","SHOP"]

    }
  },

  methods:{
    //questo metodo mi mette in collegamento l'indice che clicco con l'active index  
    //grazie a questo procedimento, la condizione per l'aggiunta della classe "Active"
    //nelle righe sotto sarà rispettata e tutti e meccanismi legati alla classe "Active"
    //entreranno in gioco
    evidenzia(linkIdex){
        this.activeLinkIndex = linkIdex
        console.log(this.activeLinkIndex)
    }
  }

}
</script>

<template>
    
    <header> 
  <div class="container1">
<img src="/img/dc-logo.png" alt="dc_logo">

<ul>
    <li v-for="(link, index) in links"   :class=" index == activeLinkIndex ? 'Active' : ''"  @mouseover="evidenzia(index)" >{{link}}</li>
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
   

 }

 li{
    position: relative;
    font-weight: bolder;
 }

 
    //e questa classe Active che mi aggiunge il comportamento in hover e il blocco blue sotto 
    //l'elemento, questa classe si aggiunge solo alla condizione stabilita sopra
    .Active:hover{
     color:$primaryColor;

    &::after{
    content: '';
    height: 10px;
    width: 100%;
    background-color:$primaryColor;
    position: absolute;
    top:50px;
    left: 0px;
   }

    }





 
</style>