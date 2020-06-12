<template>
  <div class="home">
    <img
      alt="Jhon Solier"
      src="../assets/images/avatar.jpg"
      class="main-photo"
    />
    <HelloWorld msg="¡Bienvenidos a mi página!" />
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from "@/components/HelloWorld.vue";

export default {
  name: "Home",
  components: {
    HelloWorld
  }
};
</script>

<style lang="scss" scoped>
.main-photo {
  border-radius: 50%;
}
</style>
