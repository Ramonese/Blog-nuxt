<template>
  <h1 v-if="true === true" @click="handler(arg, event)">test</h1>
</template>

<script>
export default {
  props: {
    propName: {
      type: Number,
      default: 2
    }
  }
};
</script>

<style></style>
