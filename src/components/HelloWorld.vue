<template>
  <div>
    <h1>{{ msg }}</h1>
    <p>
      Welcome to this Happyhour guide. Here you may find random links.
    </p>
    <h3>Essential Info</h3>
    <ul>
      <li><a href="http://alcoholforum.org" target="_blank">Forum</a></li>
      <li><a href="http://www.drinkingdiaries.com/about/" target="_blank">Drinking Diaries</a></li>
      <li><a href="http://drinksmixer.com" target="_blank">Drinksmixer</a></li>
    </ul>
    <h3>This will be of great interest to you!</h3>
    <ul>
      <li><a href="http://www.vuebarandrestaurant.com/" target="_blank">Vue Bar</a></li>
      <li><a href="https://www.drinkka.com/" target="_blank">Drinkers Devtools</a></li>
      <li><a href="https://www.youtube.com/watch?v=7HaW8TjGb6o" target="_blank">Beerloader</a></li>
      <li><a href="https://www.youtube.com/watch?v=2CYIxlp4e6A" target="_blank">Beeropener</a></li>
    </ul>
    <h3>Don't forget to check out the One18 bar. Click below!</h3>
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

<style scoped>
h3 {
  margin: 40px 0 0;
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
</style>
