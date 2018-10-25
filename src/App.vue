<template>
  <div id="app" class="container">
    <Profile user-name="TEST" />
  </div>
</template>

<script>
import Profile from "./components/Profile.vue";

export default {
  name: 'app',
  components: {
    Profile
    }
};

</script>

<style lang="less">
#app {
  height: 100%,
}
.container {
  font-family: sans-serif;
  @media screen and (min-width: 768px) {
    width: 750px;
    margin:0 auto;
  }
}
</style>
