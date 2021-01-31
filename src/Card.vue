<template>
  <div>
    <div class="flex w-full" :class="dark ? 'text-gray-300' : 'text-white'">
      <!-- avatar -->
      <div></div>
      <div>
        <p></p>
        <p></p>
      </div>
    </div>
    <div class="font-bold"></div>
    <div class="font-light"></div>
  </div>
</template>

<script>
export default {
  name: "Card",
  props: {
    'dark': {
      default: true
    }
  }
}
</script>

<style scoped>

</style>
