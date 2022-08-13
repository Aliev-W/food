<template>
  <TheNavbar />
  <router-view/>
  <TheFooter />
</template>

<script>
import TheNavbar from './components/TheNavbar.vue'
import TheFooter from './components/TheFooter.vue'

export default {
  name: 'App',
  components: { TheNavbar, TheFooter }
}
</script>
<style lang="scss">
@import url(https://fonts.googleapis.com/css?family=Roboto:400,500);
@import url(https://fonts.googleapis.com/css?family=Philosopher:700);

*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Roboto', 'Philosopher' sans-serif;
    scroll-behavior: smooth;
    user-select: none;
}

</style>
