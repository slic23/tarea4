<template>
  <section id="producto-datos">
      <h1>Asus ROG Strix G15 G513IC-HN003 AMD Ryzen 7 4800H/16GB/512GB SSD/RTX 3050/15.6"</h1>
      <h2> 989€</h2>
      <div class="wrapper">
          <button class="btn" @click="cambiarContador('-1')" type="button" name="button">-</button>
          <input class="cantidad" type="text" name="name" :value="contador">
          <button class="btn" @click="cambiarContador('1')" type="button" name="button">+</button>
      </div>
      <br>
      <button  class="boton"><span class="material-icons">shopping_cart</span> AÑADIR CARRITO</button>
  </section>
</template>
<script>
export default {
  Name: 'ProductoDatos',
  data () {
    return {
      contador: 1
    }
  },
  methods: {
    cambiarContador (num) {
      this.contador += +num
      if (!isNaN(this.contador) && (this.contador < 0)) {
        this.contador = 0
      }
    }
  }

}
</script>

<style scoped>
section#producto-datos {
  flex: 1 1 18rem;
}
h1 {
  font-size: 2.2rem;
}
h2 {
  font-size:1.7rem;
  color: #1abc9c;
}

.wrapper {
  height: 2rem;
  display: flex;
}

.cantidad {
  border: none;
  text-align: center;
  width: 2rem;
  font-size: 1.2rem;
  border: 1px solid #d8d8d8;
}
.btn {
  border: 1px solid #d8d8d8;
  width: 1.8rem;
}
button:focus, input:focus {
  outline: 0;
}
.boton {
background-color: blue;
}

</style>
