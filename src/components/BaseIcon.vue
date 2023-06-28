<template>
  <!-- <span class="icon" :style="{ 'font-size': size + 'px' }" v-html="iconContent"></span> -->
  {{ this.name }}
  <img src="@/assets/icons/search.svg" alt="">
  <img :src="`${ruta}`">
  <!-- <component :is="iconContent"></component> -->
</template>

<script>
export default {
  props: {
    name: {
      type: String,
      required: true,
    },
    size: {
      type: Number,
      default: 16
    },
    icon: {
      type: String,
      default: 'search'
    }
  },
  data() {
  return {
  ruta: "/src/assets/icons/search.svg"
  }
}
}
</script>

<style scoped>
.icon {
  @apply bg-slate-500 text-black  fill-current leading-none m-0 h-10 w-10;
}
</style>