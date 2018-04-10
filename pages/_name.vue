<style>
.nuxt-link-active {
  color: white;
  background: green;
}
</style>

<template>
<div>
  <div>Now on /{{ name }}</div>
  <br>
  <nuxt-link to="/test">Go to /test</nuxt-link>
  <br>
  <nuxt-link to="/测试">Go to /测试</nuxt-link>
</div>
</template>

<script>
export default {
  asyncData ({ params }) {
    return { name: params.name }
  }
}
</script>

