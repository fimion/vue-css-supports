<template>
  <div id="app" >
    <h1 class="test">{{msg}}</h1>
  </div>
</template>

<script>
export default {
  name: 'app',
  data () {
    return {
      msg: 'On desktop, this should be red. On mobile this should be blue.'
    }
  }
}
</script>

<style scoped>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

h1, h2 {
  font-weight: normal;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}

a {
  color: #42b983;
}

  .test{
    color:#0000ff;
  }
  @supports (grid-area: auto) {
    @media (min-width:1024px){
      .test{
        color:#00ff00;
      }
    }
}
@media (min-width:1024px){
  @supports (grid-area: auto) {
  .test{
    color:#ff0000;
  }
  }
}
</style>
