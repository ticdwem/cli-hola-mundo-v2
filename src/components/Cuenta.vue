<template>
  <h2>Tipo de Cuenta: {{cuenta}}</h2>
  <h2>Saldo: {{ saldo }}</h2>
  <h2> Cuenta: {{estado ? 'Activa' : 'Desactivada'}}</h2>
 <div v-for="(item, index) in servicios" :key="index">
     {{index +1}} - {{item}}
 </div>
</template>

<script>
export default {
  data() {
    return {
      saldo: 1000,
      cuenta: 'visa',
      estado: false,
      servicios: ['giro','abono','tranferencia']
    };
  },
};
</script>

<style>
</style>