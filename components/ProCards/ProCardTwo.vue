<template>
  <div class="p-4">
    <div class="p-3 px-6 w-96 flex flex-col border border-gray-50 shadow-xl rounded-md flex-1 gap-4">
      <div class="flex flex-col justify-center items-center">
        <img class="rounded-full w-14 h-14 object-cover" src="https://images.unsplash.com/photo-1534528741775-53994a69daeb?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxzZWFyY2h8NDF8fHBlcnNvbnxlbnwwfHwwfHw%3D&auto=format&fit=crop&w=800&q=60" alt="">
        <h3 class="text-lg font-semibold m-0">Helena P.</h3>
        <div class="flex space-x-1 items-center font-semibold text-yellow-400">
          <div v-for="i in 5" :key="i">
            <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="currentColor" class="w-4 h-4">
              <path fill-rule="evenodd" d="M10.788 3.21c.448-1.077 1.976-1.077 2.424 0l2.082 5.007 5.404.433c1.164.093 1.636 1.545.749 2.305l-4.117 3.527 1.257 5.273c.271 1.136-.964 2.033-1.96 1.425L12 18.354 7.373 21.18c-.996.608-2.231-.29-1.96-1.425l1.257-5.273-4.117-3.527c-.887-.76-.415-2.212.749-2.305l5.404-.433 2.082-5.006z" clip-rule="evenodd" />
            </svg>

          </div>
          <span class="text-xs">5.0</span>
        </div>
      </div>
        <div class="flex text-sm font-medium gap-4">
          <div class="px-3 py-2 space-x-1 rounded-lg bg-blue-200 text-blue-700 flex items-center text-xs font-semibold">
              <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="2" stroke="currentColor" class="w-4 h-4">
                <path stroke-linecap="round" stroke-linejoin="round" d="M3.75 13.5l10.5-11.25L12 10.5h8.25L9.75 21.75 12 13.5H3.75z" />
              </svg>
              <span>New Pro</span>
          </div>
          <div class="py-1 px-2 space-x-1 rounded-lg bg-green-200 text-green-700 flex items-center text-xs font-semibold">
            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="2" stroke="currentColor" class="w-4 h-4">
              <path stroke-linecap="round" stroke-linejoin="round" d="M9 12.75L11.25 15 15 9.75M21 12a9 9 0 11-18 0 9 9 0 0118 0z" />
            </svg>

            <span>Approved</span>
          </div>
          <div class="py-1 px-2 space-x-1 rounded-lg bg-amber-200 text-amber-700 flex items-center text-xs font-semibold">
            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="2" stroke="currentColor" class="w-4 h-4">
              <path stroke-linecap="round" stroke-linejoin="round" d="M6.633 10.5c.806 0 1.533-.446 2.031-1.08a9.041 9.041 0 012.861-2.4c.723-.384 1.35-.956 1.653-1.715a4.498 4.498 0 00.322-1.672V3a.75.75 0 01.75-.75A2.25 2.25 0 0116.5 4.5c0 1.152-.26 2.243-.723 3.218-.266.558.107 1.282.725 1.282h3.126c1.026 0 1.945.694 2.054 1.715.045.422.068.85.068 1.285a11.95 11.95 0 01-2.649 7.521c-.388.482-.987.729-1.605.729H13.48c-.483 0-.964-.078-1.423-.23l-3.114-1.04a4.501 4.501 0 00-1.423-.23H5.904M14.25 9h2.25M5.904 18.75c.083.205.173.405.27.602.197.4-.078.898-.523.898h-.908c-.889 0-1.713-.518-1.972-1.368a12 12 0 01-.521-3.507c0-1.553.295-3.036.831-4.398C3.387 10.203 4.167 9.75 5 9.75h1.053c.472 0 .745.556.5.96a8.958 8.958 0 00-1.302 4.665c0 1.194.232 2.333.654 3.375z" />
            </svg>

            <span>Elite</span>
          </div>
      </div>
      <div>
        <p class="text-center text-sm text-gray-600">Lorem ipsum dolor sit, amet consectetur adipisicing elit. Saepe veniam officiis commodi iusto esse maxime labore.</p>
      </div>
      <div class=" text-white font-semibold">
        <button class="px-3 py-2 rounded-lg w-full text-center bg-purple-700">Book</button>
      </div>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style>

</style>