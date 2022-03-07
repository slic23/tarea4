<template>
<div class="contenido">
  <div class="imagen"><img :src="image"  alt="ICONO EMPRESA"></div>
  <div class="interior"><a href="#">Home</a></div>
  <div class="interior"><a href="#">Registrarse</a></div>
  <div class="interior"><a href="#">Login</a></div>
</div>
</template>
<script>
export default {
  // eslint-disable-next-line vue/multi-word-component-names
  name: 'tabla',
  data () {
    return {
      image: require('@/assets/pcpic.png')
    }
  }
}
</script>
<style>
.contenido {
display: flex;
}
 div {
  justify-content:space-between;
  text-decoration: none;
  background-color: whitesmoke;
}
.imagen {

  margin-right: 300px;
}
img {
   width: 100px;
  height: 60px;
}

  .contenido   .interior   {
  text-decoration: none;
  color: black;
  margin: 20px;
}
a {
  text-decoration: none;
  padding: 4px;
}

.interior:hover{

background-color: blueviolet;
}
</style>
