<template>
  <div>
    <img :src="imageUrl" :alt="imageAlt" />
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
  box-sizing: border-box;
  margin: 2em 0;
  padding: 0 1em;
}
img {
  width: 100%;
  max-width: 200px;
}
p {
  font-size: 1.3em;
  text-align: justify;
}
@media (min-width: 769px) {
  div {
    padding: 0 2em;
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
    padding-left: 1em;
  }
}
</style>
