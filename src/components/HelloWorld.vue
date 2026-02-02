<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <p>
      Wikipedia <br><br>
      <a href="https://en.wikipedia.org/wiki" target="_blank" rel="noopener"></a>.
    </p>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS tozz this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
a {
  color: #42b983;
}
</style>
