<template>
  <div>
    <Tagline />
    <Form />
  </div>
</template>

<script>
    import Form from './components/Form.vue'
    import Tagline from './components/Tagline.vue'

    export default {
        name: 'App',
        components: {
          Form,
          Tagline
        }
    }
</script>

<style>
    #app {
      font-family: 'Roboto'/*, Avenir, Helvetica, Arial, sans-serif;*/;
      font-weight: 400;
      font-style: normal;
      -webkit-font-smoothing: antialiased;
      -moz-osx-font-smoothing: grayscale;
      font-size: 16px
    }
</style>
