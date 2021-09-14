<template>
  <div id="app">
    <div class="container">
      <h1 class="text-center">Vue-Translator</h1>
      <h5 class="text-center">Vue.js ile Translator</h5>
      <br />
      <div class="row">
        <div class="col-md-12 text-center">
          <searchTranslate />
        </div>
      </div>
      <div class="well">
        <h3>Arama Geçmişi</h3>
        <oldSearch />
      </div>
    </div>
  </div>
</template>

<script>
import searchTranslate from "./components/searchTranslate.vue";
import oldSearch from "./components/oldSearch.vue";
export default {
  name: "app",
  components: {
    searchTranslate,
    oldSearch
  },
  data() {
    return {
      msg: "Welcome to Your Vue.js App",
    };
  },
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

h1,
h2 {
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
</style>
