<template>
  <div>
    <section>
      <h1>
        New posts
      </h1>
      <form @submit.prevent="onSave">
        <input v-model="editedPost.title" />
        <AppButton @click="onSave">Submit</AppButton>
        <AppButton @click="onCancel">Cancel</AppButton>
      </form>
    </section>
  </div>
</template>

<script>
import AppButton from "~/components/UI/AppButton.vue";
export default {
  components: {
    AppButton
  },
  data() {
    return {
      editedPost: {
        author: "",
        title: "",
        image: "",
        content: ""
      }
    };
  },
  methods: {
    onSave() {
      console.log(this.editedPost.title);
    },
    onCancel() {
      this.$router.push("/admin");
    }
  }
};
</script>

<style lang="scss" scoped></style>
