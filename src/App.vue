<template>
  <div id="app">
  <div id="nav">
    <top-header></top-header>
  </div>
    <router-view />
  </div>
</template>
<script>
import TopHeader from '@/components/top-header';
// import { mapGetters } from "vuex";
export default {
  components: {"top-header": TopHeader},
}
// export default {
//   computed: {
//     ...mapGetters(["getSpinner"])
//   }
// };
</script>

<style lang="scss">
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
.page {
  position: absolute;
  background: rgba(0, 0, 0, 0.3);
  z-index: 25;
  width: 100%;
  height: 100%;
}
.spinner {
  z-index: 26;
  position: relative;
  top: 50%;
}
</style>
