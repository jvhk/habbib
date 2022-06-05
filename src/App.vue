<template>
  <div id="app" class=".m-auto">
    <Habbib />
  </div>
</template>

<script>
import Habbib from './components/Habbib.vue'

export default {
  name: 'App',
  components: {
    Habbib
  }
}
</script>

<style>
#app{
	display: block;
	margin: auto auto;
	width: 100%;
	height: 100%;
	max-height: 100%;
	max-width: 100%;
  width: 100%;
}
</style>
