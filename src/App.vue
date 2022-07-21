<template>   
<Navbar/>

<main>
  <router-view />
</main>

<foot />
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

<style>
main{
  margin-left: 250px
}
</style>


