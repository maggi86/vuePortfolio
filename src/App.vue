<template>
<div class="">
  <div id="navbar">
  <Navbar/>
  </div>
</div>
<foot />
<router-view />


</template>

<script>
// @ is an alias to /src
import Navbar from "./components/navbar.vue";
import foot from "./components/footer.vue";

export default {
  components: {
    Navbar,
    foot
  },
};
</script>
<style >
/* *{
        overflow: hidden !important;
} */
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  overflow-x:hidden ;
}
</style>

