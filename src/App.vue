<template>
  <main class="w-[1200px] h-[900px] bg-white rounded-[32px] shadow-lg flex [&>div]:p-8 overflow-hidden">
    <div class="sidebar-day w-1/3">
      <div class="[&>svg]:fill-blue-300 ">
        <div class="flex gap-2 relative">
          <img src="@/assets/icons/general/search.svg" class="absolute h-6 left-2 top-1/2 -translate-y-2/4" />
          <input type="text" name="searchbar" id="searchbar" placeholder="Search for places..." class="rounded-full pl-8 pr-4 w-full focus:outline-none "/>
          <button class="p-1 bg-white rounded-full hover:bg-slate-200 w-10 ease-in-out transition delay-150">
            <img src="@/assets/icons/general/location-search.svg" class="rounded-full" />
          </button>
        </div>
      </div>
      <div class="py-8">
        <img src="@/assets/icons/weather-icons/Party-cloudy.svg"/>
      </div>
      <p class="text-[72px] text-white">24°C</p>
      <p class="text-white text-xl font-medium mt-4"> Tuesday, <span>90:00PM</span></p>
      <hr class="mt-8">
      <ul class="[&>li]:flex [&>li]:gap-4 mt-8 flex flex-col gap-6 text-white text-lg">
        <li>
          <img src="@/assets/icons/weather-icons/Party-cloudy.svg" class="w-8">
          <p>Mostly Cloudy</p>
        </li>
        <li>
          <img src="@/assets/icons/weather-icons/Rain.svg" class="w-8">
          <p>Rain - 30%</p>
        </li>
      </ul>
      <p class="text-white text-2xl font-medium items-center justify-center mt-8">New York, NY, USA</p>
    </div>
    <div class="bg-[#f6f6f8] w-2/3">div2</div>
  </main>
</template>

<script>
// import BaseIcon from './components/BaseIcon.vue'

export default {
  name: 'App',
  components: {
    // BaseIcon
}
}
</script>
<style lang="postcss" scoped>
.sidebar-day{
  @apply bg-gradient-to-b from-sky-300 to-sky-600;
}
.sidebar-night{
  @apply bg-gradient-to-b from-indigo-900 to-sky-600;
}
</style>