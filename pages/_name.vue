<style>
.nuxt-link-active {
  color: white;
  background: green;
}
</style>

<template>
<div>
  <nuxt-link :to="'/' + name">{{ name }}</nuxt-link>
</div>
</template>

<script>
export default {
  asyncData ({ params }) {
    return { name: params.name }
  }
}
</script>

