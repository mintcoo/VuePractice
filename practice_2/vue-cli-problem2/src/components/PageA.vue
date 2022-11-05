<template>
  <div>
    <h1>A-page</h1>
    <p>{{ goData }}</p>
  </div>
</template>

<script>
export default {
  name: 'PageA',
  props: {
    goData: String,
  }
}
</script>

<style>

</style>