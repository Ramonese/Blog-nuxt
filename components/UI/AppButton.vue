<template>
  <button class="button" :class="btnStyle" v-bind="$attrs" v-on="$listeners">
    <slot />
  </button>
</template>

<script>
export default {
  name: "AppButton",
  props: {
    btnStyle: {
      type: String,
      default: ""
    }
  }
};
</script>

<style>
.button {
  background: none;
  color: indigo;
  padding: 1em;
  border: 1px solid black;
}
</style>
