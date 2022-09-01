<template>
  <div class=" container mx-auto">
    <div class="">
      <div class="fixed bg-white w-full top-0 flex p-4 text-lg font-mono font-semibold">
        Pro card designs
      </div>
      <div class="mt-10 flex gap-4 py-4">
        <div class="flex flex-col overflow-auto">
          <ProCardOne v-for="i in 4" :key="i" />
        </div>
        <div class="flex flex-col">
          <ProCardTwo v-for="i in 4" :key="i" />
        </div>
        <div class="flex flex-col">
          <ProCardThree v-for="i in 4" :key="i" />
        </div>
      </div>
    </div>
  </div>
</template>

<script>


export default {
  
}
</script>