<template>
  <navegador />
  <cuerpoPagina />
  <crumbNavegation/>
  <div class="contenido">

    <div>
  <productoImagen/>
  </div>

 <div class="espacio"> <LateralCompra/></div>
</div>
<videoDescriptivo/>
<pieStore/>
</template>
<script>
import Navegador from '@/components/Navegador.vue'
import cuerpoPagina from '@/components/cuerpoPagina.vue'
import crumbNavegation from '@/components/crumbNavegation.vue'
import productoImagen from '@/components/productoImagen.vue'
import LateralCompra from '@/components/LateralCompra.vue'
import VideoDescriptivo from '@/components/VideoDescriptivo.vue'
import PieStore from '@/components/PieStore.vue'
export default {
  name: 'App',
  components: {
    Navegador,
    cuerpoPagina,
    crumbNavegation,
    productoImagen,
    LateralCompra,
    VideoDescriptivo,
    PieStore
  }
}
</script>
<style scoped>
.contenido {
display: flex;
}
</style>
