<template>
  <section class="container">
    <div>
      {{ $route.params }}
    </div>
  </section>
</template>

<script>
export default {
  validate ({ params }) {
    // 数値でなければならない
    return /^\d+$/.test(params.id)
  }
}
</script>

<style>
</style>
