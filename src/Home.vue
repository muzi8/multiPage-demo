<template>
  <div id="app" :class="{'header-hide': headerHide}">
    This is my {{ name }}
  </div>
</template>

<script>
export default {
  data () {
    return {
      name: 'home'
    }
  }
}
</script>

<style>

</style>
