<template>
  <h1>user id is: {{ $route.params.id }}</h1>
</template>

<script>
    export default {
      validate ({params}) {
      //  Number
        return /^\d+$/.test(params.id)
      },
        name: "index"
    }
</script>

<style scoped>

</style>
