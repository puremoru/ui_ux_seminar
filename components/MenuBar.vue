<template>
  <div class="inline-block">
    <div class="absolute h-screen bg-indigo-900 w-20" style="z-index: -1;"></div>
      <div class="flex">
        <div class="flex bg-sidebar">
          <ul class="flex list-none h-full flex-col text-white text-center">
            <li class="p-4 btn-sidebar cursor-pointer text-xs">
              <div class="flex items-center justify-center">
                <svg class="h-8 w-8 text-white"  viewBox="0 0 20 20" fill="currentColor">  <path d="M10 2a6 6 0 00-6 6v3.586l-.707.707A1 1 0 004 14h12a1 1 0 00.707-1.707L16 11.586V8a6 6 0 00-6-6zM10 18a3 3 0 01-3-3h6a3 3 0 01-3 3z"/></svg>
              </div>
              最新情報</li>
            <li class="p-4 btn-sidebar cursor-pointer text-xs">
              <div class="flex items-center justify-center">
                <svg class="h-8 w-8 text-white"  viewBox="0 0 20 20" fill="currentColor">  <path fill-rule="evenodd" d="M18 5v8a2 2 0 01-2 2h-5l-5 4v-4H4a2 2 0 01-2-2V5a2 2 0 012-2h12a2 2 0 012 2zM7 8H5v2h2V8zm2 0h2v2H9V8zm6 0h-2v2h2V8z" clip-rule="evenodd"/></svg>
              </div>
              チャット</li>
            <li class="p-4 btn-sidebar cursor-pointer text-xs">
              <div class="flex items-center justify-center">
                <svg class="h-8 w-8 text-white"  viewBox="0 0 20 20" fill="currentColor">  <path d="M13 6a3 3 0 11-6 0 3 3 0 016 0zM18 8a2 2 0 11-4 0 2 2 0 014 0zM14 15a4 4 0 00-8 0v3h8v-3zM6 8a2 2 0 11-4 0 2 2 0 014 0zM16 18v-3a5.972 5.972 0 00-.75-2.906A3.005 3.005 0 0119 15v3h-3zM4.75 12.094A5.973 5.973 0 004 15v3H1v-3a3 3 0 013.75-2.906z"/></svg>
              </div>
              チーム</li>
            <li class="p-4 btn-sidebar cursor-pointer text-xs">
              <div class="flex items-center justify-center">
                <svg class="h-8 w-8 text-white"  viewBox="0 0 20 20" fill="currentColor">  <path d="M9 2a1 1 0 000 2h2a1 1 0 100-2H9z"/>  <path fill-rule="evenodd" d="M4 5a2 2 0 012-2 3 3 0 003 3h2a3 3 0 003-3 2 2 0 012 2v11a2 2 0 01-2 2H6a2 2 0 01-2-2V5zm3 4a1 1 0 000 2h.01a1 1 0 100-2H7zm3 0a1 1 0 000 2h3a1 1 0 100-2h-3zm-3 4a1 1 0 100 2h.01a1 1 0 100-2H7zm3 0a1 1 0 100 2h3a1 1 0 100-2h-3z" clip-rule="evenodd"/></svg>
              </div>
              課題</li>
            <li class="p-4 btn-sidebar cursor-pointer text-xs">
              <div class="flex items-center justify-center">
                <svg class="h-8 w-8 text-white"  viewBox="0 0 24 24" stroke-width="2" stroke="currentColor" fill="none" stroke-linecap="round" stroke-linejoin="round">  <path stroke="none" d="M0 0h24v24H0z"/>  <rect x="4" y="5" width="16" height="16" rx="2" />  <line x1="16" y1="3" x2="16" y2="7" />  <line x1="8" y1="3" x2="8" y2="7" />  <line x1="4" y1="11" x2="20" y2="11" />  <rect x="8" y="15" width="2" height="2" /></svg>
              </div>
              予定表</li>
            <li class="p-4 btn-sidebar cursor-pointer text-xs">
              <div class="flex items-center justify-center">
                <svg class="h-8 w-8 text-white"  viewBox="0 0 20 20" fill="currentColor">  <path d="M2 3a1 1 0 011-1h2.153a1 1 0 01.986.836l.74 4.435a1 1 0 01-.54 1.06l-1.548.773a11.037 11.037 0 006.105 6.105l.774-1.548a1 1 0 011.059-.54l4.435.74a1 1 0 01.836.986V17a1 1 0 01-1 1h-2C7.82 18 2 12.18 2 5V3z"/></svg>
              </div>
              通話</li>
            <li class="p-4 btn-sidebar cursor-pointer text-xs">
              <div class="flex items-center justify-center">
                <svg class="h-8 w-8 text-white"  viewBox="0 0 20 20" fill="currentColor">  <path fill-rule="evenodd" d="M4 4a2 2 0 012-2h4.586A2 2 0 0112 2.586L15.414 6A2 2 0 0116 7.414V16a2 2 0 01-2 2H6a2 2 0 01-2-2V4z" clip-rule="evenodd"/></svg>
              </div>
              ファイル</li>
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
