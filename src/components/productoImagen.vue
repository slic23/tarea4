<template>
  <section id="producto-imagen">
      <div class="img-big">
          <img  class="imagen_grande" v-bind:src="fotos[0]" alt="iMAGEN 1">
      </div>
        <div class="img-mini">
          <a @click="cambiarFoto(1)"><img  v-bind:src="fotos[1]" alt="GT"></a>
          <a @click="cambiarFoto(2)"><img  v-bind:src="fotos[2]" alt="iMAGEN 2"></a>
          <a @click="cambiarFoto(3)"><img  v-bind:src="fotos[3]" alt="iMAGEN 3"></a>
        </div>
      </section>
</template>

<script>
export default {
  Name: 'ProductoImagen',
  data () {
    return {
      fotos: [
        require('../assets/principal.webp'),
        require('../assets/p1.png'),
        require('../assets/p2.png'),
        require('../assets/p3.png'),
        require('../assets/p4.png')]
    }
  },
  methods: {
    cambiarFoto (id) {
      this.fotos[0] = this.fotos[id]
    }
  }

}
</script>

<style >

section {
    margin-left: 50px;
}

.imagen_grande{

    width: 500px;
    height: 400px;
}

</style>
