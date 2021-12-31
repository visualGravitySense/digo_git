<template>
  <div class="posts">
    <input type="text" v-model="postId">
    <button @click="loadPost"> Get Post </button>
  </div>
</template>

<script>
  export default {
    data () {
      return {
        postId: ''
      }
    },
    methods: {
      loadPost () {
        this.$router.push(`/posts/${this.postId}`)
      }
    },
    name: "index"
  }
</script>

<style scoped>

</style>
