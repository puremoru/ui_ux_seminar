<template>
  <div>
    <div class="h-12 bg-indigo-800">
      <div class="flex h-full">
        <div class="flex w-full items-center justify-center">
          <svg
            class="h-5 w-5 text-gray-200 mx-1"
            fill="none"
            viewBox="0 0 24 24"
            stroke="currentColor"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              d="M15 19l-7-7 7-7"
            />
          </svg>
          <svg
            class="h-5 w-5 text-gray-500 mx-1"
            fill="none"
            viewBox="0 0 24 24"
            stroke="currentColor"
          >
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 5l7 7-7 7" />
          </svg>
          <svg
            class="h-5 w-5 text-gray-300 mx-4"
            fill="none"
            viewBox="0 0 24 24"
            stroke="currentColor"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              d="M11 5H6a2 2 0 00-2 2v11a2 2 0 002 2h11a2 2 0 002-2v-5m-1.414-9.414a2 2 0 112.828 2.828L11.828 15H9v-2.828l8.586-8.586z"
            />
          </svg>
          <input
            class="w-1/2 shadow rounded py-2 px-3 bg-orange-100 placeholder-gray-700 text-xs"
            type="search"
            placeholder="人、キーワードの検索、またはコマンドの入力"
          />
        </div>
        <div class="flex items-center ml-auto mr-2">
          <svg class="h-8 w-8 text-gray-400" fill="none" viewBox="0 0 24 24" stroke="currentColor">
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              d="M5.121 17.804A13.937 13.937 0 0112 16c2.5 0 4.847.655 6.879 1.804M15 10a3 3 0 11-6 0 3 3 0 016 0zm6 2a9 9 0 11-18 0 9 9 0 0118 0z"
            />
          </svg>
        </div>
      </div>
    </div>
    <nuxt />
  </div>
</template>

<script>
import MenuBar from "~/components/MenuBar.vue";
export default {
  components: {
    MenuBar
  }
};
</script>
