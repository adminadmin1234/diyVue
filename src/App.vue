<template>
  <div>
    <div class="App">
        <img :src="imgUrl1">
        <div>Hello {{msg}}</div>
    </div>
    <div>
        <router-link to="/page1">go page1</router-link>
        <router-link to="/page2">go page2</router-link>
        </div>
        <div>
        <router-view></router-view>
        </div>
    </div>
</template>
<script>
export default {
  name: 'App',

  data() {
    return {
        msg: "diyVue",
        imgUrl1: require('./assets/logo.png'),
    };
  }
};
</script>
<style lang="scss" scoped>
    .App{
        color:red;
    }
</style>
