<template>
  <form @submit.prevent="onSave">
    <AppInput v-model="editedPost.title">Post title</AppInput>
    <AppInput v-model="editedPost.author">Post author</AppInput>
    <AppInput v-model="editedPost.image">Post image</AppInput>
    <AppInput control-type="textarea" v-model="editedPost.content"
      >Text</AppInput
    >
    <AppButton @click="onSave">Submit</AppButton>
    <AppButton @click="onCancel">Cancel</AppButton>
  </form>
</template>

<script>
import AppButton from "~/components/UI/AppButton.vue";
import AppInput from "~/components/UI/AppInput.vue";
export default {
  components: {
    AppButton,
    AppInput
  },
  props: {
    post: {
      type: Object,
      required: false
    }
  },
  data() {
    return {
      editedPost: this.post
        ? { ...this.post }
        : {
            author: "",
            title: "",
            image: "",
            content: ""
          }
    };
  },
  methods: {
    onSave() {
      console.log(this.editedPost);
    },
    onCancel() {
      this.$router.push("/admin");
    }
  }
};
</script>

<style>
section.form {
  max-width: 90ch;
  margin: auto;
}
form label {
  display: block;
  color: magenta;
}
</style>
