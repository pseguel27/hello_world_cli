<template>
  <button @click="accion()" :disabled="desactivar">{{label}}</button>
</template>

<script>
export default {
  props: {
    label:String,
    desactivar: {
      type:Boolean,
      default: false
    }
  },
  methods: {
    accion(){
      this.$emit('accion')
    }
  }
}
</script>

<style>

</style>