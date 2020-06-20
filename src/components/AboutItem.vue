<template>
  <div>
    <img :src="require('@/assets/images/' + imageUrl)" :alt="imageAlt" />
    <p>{{ text }}</p>
  </div>
</template>

<script lang="ts">
import { Component, Prop, Vue } from "vue-property-decorator";

@Component
export default class AboutItem extends Vue {
  @Prop() private imageUrl!: string;
  @Prop() private imageAlt!: string;
  @Prop() private text!: string;
}
</script>

<style lang="scss" scoped>
div {
  margin: 2em 0;
}
img,
p {
  display: inline-block;
  vertical-align: middle;
}
img {
  width: 15%;
}
p {
  box-sizing: border-box;
  width: 85%;
  margin: 0;
  padding-left: 2em;
  text-align: left;
  font-size: 1.3em;
}
</style>
