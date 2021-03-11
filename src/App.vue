<template>
  <div id="app">
    <Header msg="Physio"/>
  </div>
</template>

<script>
import Header from './components/Header.vue'

export default {
  name: 'App',
  components: {
    Header
  }
}
</script>

<style>
:root
{
  --firstColor:#1D3557;
  --secondColor:#ffffff;
  --thirdColor:#A8DADC;
  --forthColor:#457B9D;
  --fifthColor:#1D3557;
  --navActive:#a7b7c7;
  --navInactive:#677788;
  --navActiveFocus: var(--firstColor);
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  display: block;
}

body{
  margin:0;
}

</style>
