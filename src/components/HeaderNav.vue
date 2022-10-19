<template>
  <div class="title">This's my demo with vue3</div>
  <button @click="onAdd">Toggle message</button>
  <div v-if="isShow">{{ msg }}</div>
</template>

<script>
import { defineComponent } from "vue";

export default defineComponent({
  name: "HeaderNav",
  data() {
    return {
      msg: "Hello, my name's HN",
      isShow: false,
    };
  },
  methods: {
    onAdd() {
      this.isShow = !this.isShow;
    },
  },
});
</script>

<style lang="scss">
.title {
  color: lightsteelblue;
}
</style>
