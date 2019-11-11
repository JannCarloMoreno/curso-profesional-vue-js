<template lang="pug">
  #app
    input(v-model="name")
    p {{name}}

    a(v-bind:href="url" target="_blank") link
</template>

<script>
export default {
  name: 'app',
  data () {
    return {
      name: '',
      url: 'http://platzi.com'
    }
  }
}
</script>

<style lang="scss">
@import './scss/main.scss';
</style>
