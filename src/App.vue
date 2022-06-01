<template>
  <div class="">
    <h1>{{inputtext}}  </h1>
    <h2 :class="claseprueba" v-text="texto"></h2>
    <p v-html="textohtm2"></p>  
    <input type="text" v-model="inputtext">
    <img :src="image" alt="">
  </div>
</template>
<script>
export default {
  name: "App",
  data(){
    return{
      mensaje:"hola vuevue",
      texto:"hola mundo",
      textohtml:"<h1>otra frase</h1>",
      textohtm2:'<a href="https://google.com">otra frase</h1>',
      inputtext:"Escribre un texto",
      image:"https://picsum.photos/200/300",
      claseprueba:"texto-rojo"
    }
  },
}
</script>
<style>
.texto-azul{
  color: blue;
}
.texto-rojo{
  color:red;
  background-color: black;
}

</style>
