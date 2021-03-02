<template>
  <HelloWorld />
  <FriendDetails />
  <FriendDetails />
  <FriendDetails />
  <FriendDetails />
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";
import Friend from "./components/Friend.vue";

export default {
  name: "App",
  components: {
    HelloWorld,
    FriendDetails: Friend,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
