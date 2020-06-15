<template>
  <div class="inline-block">
    <div class="absolute h-screen bg-indigo-900 w-20" style="z-index: -1;"></div>
      <div class="flex">
        <div class="flex bg-sidebar">
          <ul class="flex list-none h-full flex-col text-white text-center">
            <li class="p-4 btn-sidebar cursor-pointer text-xs">最新情報</li>
            <li class="p-4 btn-sidebar cursor-pointer text-xs">チャット</li>
            <li class="p-4 btn-sidebar cursor-pointer text-xs">チーム</li>
            <li class="p-4 btn-sidebar cursor-pointer text-xs">課題</li>
            <li class="p-4 btn-sidebar cursor-pointer text-xs">予定表</li>
            <li class="p-4 btn-sidebar cursor-pointer text-xs">通話</li>
            <li class="p-4 btn-sidebar cursor-pointer text-xs">ファイル</li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</template>

<style>
  .bg-sidebar {
  	/* background-color: rgba(255, 255, 255, 0.6); */
  }

  .btn-sidebar:hover {
    background-color: rgba(255, 255, 255, 0.25);
  }

  .bg-content {
    background-color: rgba(255, 255, 255, 0.85);
  }
</style>
