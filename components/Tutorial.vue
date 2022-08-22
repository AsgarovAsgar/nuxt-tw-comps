<!-- Please remove this file from your project -->
<template>
  <div class="flex items-top justify-center min-h-screen bg-gray-100 sm:items-center sm:pt-0">
    <div class="relative">
      <button @click="showDropdown" id="dropdownBgHoverButton" data-dropdown-toggle="dropdownBgHover" class="text-white bg-blue-700 hover:bg-blue-800 focus:ring-4 focus:outline-none focus:ring-blue-300 font-medium rounded-lg text-sm px-4 py-2.5 text-center inline-flex items-center dark:bg-blue-600 dark:hover:bg-blue-700 dark:focus:ring-blue-800" type="button">Dropdown checkbox <svg class="ml-2 w-4 h-4" aria-hidden="true" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 9l-7 7-7-7"></path></svg></button>

    <!-- Dropdown menu -->
      <transition
        enter="transition-opacity duration-75"
        enterFrom="opacity-0"
        enterTo="opacity-100"
        leave="transition-opacity duration-150"
        leaveFrom="opacity-100"
        leaveTo="opacity-0"
      >
      <div v-show="isOpen" id="dropdownBgHover" class="absolute top-12 z-10 bg-white rounded shadow dark:bg-gray-700 block" data-popper-reference-hidden="" data-popper-escaped="" data-popper-placement="bottom">
          <ul class="p-3 space-y-1 text-sm text-gray-700 dark:text-gray-200" aria-labelledby="dropdownBgHoverButton">
            <li>
              <label for="checkbox-item-1" class="flex items-center p-2 rounded hover:bg-gray-100 dark:hover:bg-gray-600 cursor-pointer transition duration-200">
                <input checked="" id="checkbox-item-1" type="checkbox" value="" class="w-4 h-4 text-blue-600 bg-gray-100 rounded border-gray-300 focus:ring-blue-500 dark:focus:ring-blue-600 dark:ring-offset-gray-700 focus:ring-2 dark:bg-gray-600 dark:border-gray-500">
                <span  class="ml-2 w-full text-sm font-medium text-gray-900 rounded dark:text-gray-300">Dashboard</span>
              </label>
            </li>
            <li>
              <label for="checkbox-item-2" class="flex items-center p-2 rounded hover:bg-gray-100 dark:hover:bg-gray-600 cursor-pointer transition duration-200">
                <input checked="" id="checkbox-item-2" type="checkbox" value="" class="w-4 h-4 text-blue-600 bg-gray-100 rounded border-gray-300 focus:ring-blue-500 dark:focus:ring-blue-600 dark:ring-offset-gray-700 focus:ring-2 dark:bg-gray-600 dark:border-gray-500">
                <span  class="ml-2 w-full text-sm font-medium text-gray-900 rounded dark:text-gray-300">Checked state</span>
              </label>
            </li>
            <li>
              <label for="checkbox-item-5" class="flex items-center p-2 rounded hover:bg-gray-100 dark:hover:bg-gray-600 cursor-pointer transition duration-200">
                <input checked="" id="checkbox-item-5" type="checkbox" value="" class="w-4 h-4 text-blue-600 bg-gray-100 rounded border-gray-300 focus:ring-blue-500 dark:focus:ring-blue-600 dark:ring-offset-gray-700 focus:ring-2 dark:bg-gray-600 dark:border-gray-500">
                <span  class="ml-2 w-full text-sm font-medium text-gray-900 rounded dark:text-gray-300">Additional information</span>
              </label>
            </li>
          </ul>
      </div>
      </transition>
    </div>
  </div>
</template>

<script>
export default {
  name: 'NuxtTutorial',
  data() {
    return {
      isOpen: false,
      result: 'here'
    };
  },
  mounted() {

  },
  methods: {
    showDropdown() {
      this.isOpen = !this.isOpen
      let word = 'javascripot'
      let sait = 'ai'
      let wordVowels = []
      let wordSamits = []
      for(let w of word) {
        if(sait.includes(w)) {
          wordVowels.push(w)
        } else {
          wordSamits.push(w)
        }
      }
      let result = [...wordVowels, ...wordSamits]
      console.log('result', result);
    }
  }
}
</script>
