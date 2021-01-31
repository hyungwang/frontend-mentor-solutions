<template>
  <div class="app py-40 space-y-32 min-h-screen w-screen bg-gradient-to-br from-green-300 to-blue-600 flex flex-col justify-center items-center">
    <div class="bg-white w-96 overflow-hidden rounded-2xl shadow-2xl">
      <div class="h-40 w-full bg-gradient-to-br from-green-500 to-blue-900"></div>
      <div class="bg-gray-500 border-4 border-white shadow-md -mt-12 h-24 w-24 mx-auto rounded-full">

      </div>
      <div class="py-10 space-y-3 text-center">
        <div class="flex justify-center whitespace-nowrap space-x-5 items-center">
          <h5 class="text-gray-700 font-bold">Victor Crest</h5>
          <span class="text-gray-400 text-sm">26</span>
        </div>
        <p class="font-light text-gray-700 text-sm">
          London
        </p>
      </div>
      <div class="border-t border-gray-100  flex justify-around py-3">
        <div v-for="f in footer" class="flex flex-col items-center w-20">
          <span class="font-extrabold text-lg">{{ f.value }}</span>
          <span class="text-xs text-gray-400">{{ f.title }}</span>
        </div>
      </div>
    </div>


    <div class=" w-3/5 gap-x-4 gap-y-6 grid grid-cols-4 grid-rows-2 h-96  my-5">
      <div class="col-start-1 col-end-3 row-start-1 row-end-2 bg-purple-400 rounded-xl shadow-xl">
        <Card :dark="false"/>
      </div>
      <div class="col-start-3 col-end-4 row-start-1 row-end-2 bg-gray-500 rounded-xl shadow-xl">
        <Card/>
      </div>
      <div class="col-start-4 col-end-5 row-start-1 row-end-3 bg-white rounded-xl shadow-xl">
        <Card/>
      </div>
      <div class="col-start-1 col-end-2 bg-white rounded-xl shadow-xl">
        <Card/>
      </div>
      <div class="col-start-2 col-end-4 row-start-2 row-end-3 bg-gray-900 rounded-xl shadow-xl">
        <Card/>
      </div>
    </div>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import Card from "@/Card";

export default {
  name: 'App',
  components: {
    Card,
    HelloWorld
  },
  data() {
    return {
      footer: [
        {
          title: 'Followers',
          value: '80K'
        },
        {
          title: 'Likes',
          value: '803K'
        },
        {
          title: 'Photos',
          value: '1.4K'
        }
      ]
    }
  }
}
</script>

<style lang="scss">

</style>
