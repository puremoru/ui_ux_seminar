<template>
  <div>
    <MenuBar />
    <div class="inline-block absolute ">
      <div class="w-full border shadow h-screen">
	      <div class="flex">
            <!-- Sidebar / channel list -->
            <div class="text-purple-lighter pb-6 hidden md:block">
              <div class="flex items-center mb-6 px-4 mt-5 border-b">
                <span class="bg-green rounded-full block w-2 h-2"></span>
                <span class="text-purple-lightest text-xl font-bold">チャット</span>
                <span class="ml-16 text-sm text-indigo-800">最近</span>
                <span class="ml-3 text-sm">連絡先</span>
                <span class="ml-8"><svg class="h-5 w-5 text-black"  width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><polygon points="22 3 2 3 10 12.46 10 19 14 21 14 12.46 22 3"></polygon></svg></span>
              </div>
              <div>
                <span class="ml-3 text-xs">最近のチャット</span>
              </div>
              <div class="bg-gray-300 h-16 mt-5 flex items-center">
                <div class="ml-3 rounded-full">
                  <!-- <span class="bg-purple-200 align-middle">城</span> -->
                  <svg  width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-user h-8 w-8 text-gray-500"><path d="M20 21v-2a4 4 0 0 0-4-4H8a4 4 0 0 0-4 4v2"></path><circle cx="12" cy="7" r="4"></circle></svg>
                </div>
                <div class="ml-2">
                  <span>城後 明慈</span>
                </div>
                <div class="flex ml-32 text-sm">
                  <span>06/09</span>
                </div>
              </div>
            </div>

            <!-- Chat content -->
            <div class="bg-gray-200 flex flex-col h-screen">
                <!-- Top bar -->
                <div class="border-b flex px-6 py-2 items-center">
                    <div class="flex">
                        <div class="rounded-full h-4 w-4">
                          <svg  width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-user h-8 w-8 text-gray-500"><path d="M20 21v-2a4 4 0 0 0-4-4H8a4 4 0 0 0-4 4v2"></path><circle cx="12" cy="7" r="4"></circle></svg>
                        </div>
                        <h3 class="text-grey-darkest text-lg mb-1 font-extrabold flex-initial px-1 ml-6">城後 明慈</h3>
                        <h3 class="text-grey-darkest text-base ml-2 mb-1 flex-initial px-1 font-bold text-indigo-800">チャット</h3>
                        <h3 class="text-grey-darkest text-base ml-2 mb-1 flex-initial px-1">ファイル</h3>
                        <h3 class="text-grey-darkest text-base ml-2 mb-1 flex-initial px-1">組織</h3>
                        <h3 class="text-grey-darkest text-base ml-2 mb-1 flex-initial px-1">最新情報</h3>
                        <h3 class="text-grey-darkest text-base ml-2 mb-1 flex-initial px-1">＋</h3>
                    </div>
                    <div class="ml-auto hidden md:block">
                        <div class="flex">
                          <svg class="px-1 h-8 w-8 text-indigo-700" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><polygon points="23 7 16 12 23 17 23 7"></polygon><rect x="1" y="5" width="15" height="14" rx="2" ry="2"></rect></svg>
                          <svg class="px-1 h-8 w-8 text-indigo-700" viewBox="0 0 24 24" stroke-width="2" stroke="currentColor" fill="none" stroke-linecap="round" stroke-linejoin="round">  <path stroke="none" d="M0 0h24v24H0z"/>  <path d="M4 4h5l2 5l-2.5 1.5a11 11 0 0 0 5 5l1.5 -2.5l5 2v5a1 1 0 0 1 -1 1a16 16 0 0 1 -16 -16a1 1 0 0 1 1 -1" /></svg>
                          <div class="grid grid-cols-2 divide-x divide-gray-400">
                            <svg class="px-1 h-8 w-8 text-indigo-700 text-center" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M5 17H4a2 2 0 0 1-2-2V5a2 2 0 0 1 2-2h16a2 2 0 0 1 2 2v10a2 2 0 0 1-2 2h-1"></path><polygon points="12 15 17 21 7 21 12 15"></polygon></svg>
                            <svg class="px-1 h-8 w-8 text-black text-center"  width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M16 21v-2a4 4 0 0 0-4-4H5a4 4 0 0 0-4 4v2"></path><circle cx="8.5" cy="7" r="4"></circle><line x1="20" y1="8" x2="20" y2="14"></line><line x1="23" y1="11" x2="17" y2="11"></line></svg>
                          </div>
                          <svg class="px-1 flex-initial h-8 w-8 text-black"  fill="none" viewBox="0 0 24 24" stroke="currentColor">
  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M10 6H6a2 2 0 00-2 2v10a2 2 0 002 2h10a2 2 0 002-2v-4M14 4h6m0 0v6m0-6L10 14"/>
</svg>
                        </div>
                    </div>
                </div>

          <!-- Chat messages -->
                <div class="px-6 py-4 flex-1 overflow-scroll-x">
                  <!-- A message -->
                    <div class="flex items-start mb-4">
                        <!-- <img src="https://avatars2.githubusercontent.com/u/343407?s=460&v=4" class="w-10 h-10 rounded mr-3" /> -->
                        <div class="rounded-full h-4 w-4">
                          <svg  width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-user h-8 w-8 text-gray-500"><path d="M20 21v-2a4 4 0 0 0-4-4H8a4 4 0 0 0-4 4v2"></path><circle cx="12" cy="7" r="4"></circle></svg>
                        </div>
                        <div class="flex flex-col ml-6 bg-white">
                            <div class="flex items-end mx-4 mt-2">
                              <span class="text-md mr-2 font-sans">城後 明慈</span>
                              <span class="text-grey ml-auto text-gray-600 text-sm font-light">05/12 11:46</span>
                            </div>
                          <p class="font-light text-md text-grey-darkest pt-1 mx-4 my-2">やあ！いぶきくん！今日もいい朝だね！</p>
                        </div>
                    </div>

                    <div class="flex items-start mb-4 justify-end">
                        <div class="flex flex-col ml-6 bg-indigo-100">
                            <div class="flex items-end mx-4 mt-2">
                              <span class="text-grey text-gray-600 text-sm font-light">05/12 16:56</span>
                            </div>
                          <p class="font-light text-md text-grey-darkest pt-1 mx-4 my-2">おはよう</p>
                        </div>
                    </div>

                    <div class="flex items-start mb-4">
                        <!-- <img src="https://avatars2.githubusercontent.com/u/343407?s=460&v=4" class="w-10 h-10 rounded mr-3" /> -->
                        <div class="rounded-full h-4 w-4">
                          <svg  width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-user h-8 w-8 text-gray-500"><path d="M20 21v-2a4 4 0 0 0-4-4H8a4 4 0 0 0-4 4v2"></path><circle cx="12" cy="7" r="4"></circle></svg>
                        </div>
                        <div class="flex flex-col ml-6 bg-white">
                            <div class="flex items-end mx-4 mt-2">
                              <span class="text-md mr-2 font-sans">城後 明慈</span>
                              <span class="text-grey ml-auto text-gray-600 text-sm font-light">05/12 16:56</span>
                            </div>
                          <p class="font-light text-md text-grey-darkest pt-1 mx-4 my-2">今日は何して過ごしてたの？？</p>
                        </div>
                    </div>

                    <div class="flex items-start mb-4 justify-end">
                        <div class="flex flex-col ml-6 bg-indigo-100">
                            <div class="flex items-end mx-4 mt-2">
                              <span class="text-grey text-gray-600 text-sm font-light">05/13 14:02</span>
                            </div>
                          <p class="font-light text-md text-grey-darkest pt-1 mx-4 my-2">ごめん、寝てた。</p>
                        </div>
                    </div>
                    

                    <!-- A message -->
                    <div class="flex items-start">
                        <div class="flex flex-col">
                            <div class="flex items-end">
                              <span class="font-bold text-md mr-2 font-sans text-gray-200">Adam Bishop</span>
                              <span class="text-grey text-xs font-light text-gray-200">12:46</span>
                            </div>
                          <p class="font-light text-md text-grey-darkest pt-1 text-gray-200"><a href="#" class="text-blue">@Olivia Dunham</a> the size of the generated CSS is creating a singularity in space/time, we must stop adding more utilities before it's too late!aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa..</p>
                        </div>
                    </div>

                </div>

                <div class="m-12">
                  <div class="flex rounded-lg border-2 border-grey overflow-hidden">
                    <!-- <span class="text-3xl text-grey px-3 border-r-2 border-grey">+</span> -->
                    <input type="text" class="w-full px-4 h-10" placeholder="新しいメッセージの入力"/>
                  </div>
                  <div>
                    <ul class="flex rounded-lg overflow-hidden">
                      <li class="p-4 btn-sidebar cursor-pointer text-xs">
                        <div class="flex items-center justify-center">
                          <svg class="h-4 w-4 text-black"  viewBox="0 0 24 24" stroke-width="2" stroke="currentColor" fill="none" stroke-linecap="round" stroke-linejoin="round">  <path stroke="none" d="M0 0h24v24H0z"/>  <polyline points="16 4 20 4 20 8" />  <line x1="14" y1="10" x2="20" y2="4" />  <polyline points="8 20 4 20 4 16" />  <line x1="4" y1="20" x2="10" y2="14" /></svg>
                        </div>
                      </li>
                      <li class="p-4 btn-sidebar cursor-pointer text-xs">
                        <div class="flex items-center justify-center">
                          <svg class="h-4 w-4 text-black"  viewBox="0 0 20 20" fill="currentColor">  <path fill-rule="evenodd" d="M18 3a1 1 0 00-1.447-.894L8.763 6H5a3 3 0 000 6h.28l1.771 5.316A1 1 0 008 18h1a1 1 0 001-1v-4.382l6.553 3.276A1 1 0 0018 15V3z" clip-rule="evenodd"/></svg>
                        </div>
                      </li>
                      <li class="p-4 btn-sidebar cursor-pointer text-xs">
                        <div class="flex items-center justify-center">
                          <svg class="h-4 w-4 text-black"  viewBox="0 0 20 20" fill="currentColor">  <path fill-rule="evenodd" d="M12.586 4.586a2 2 0 112.828 2.828l-3 3a2 2 0 01-2.828 0 1 1 0 00-1.414 1.414 4 4 0 005.656 0l3-3a4 4 0 00-5.656-5.656l-1.5 1.5a1 1 0 101.414 1.414l1.5-1.5zm-5 5a2 2 0 012.828 0 1 1 0 101.414-1.414 4 4 0 00-5.656 0l-3 3a4 4 0 105.656 5.656l1.5-1.5a1 1 0 10-1.414-1.414l-1.5 1.5a2 2 0 11-2.828-2.828l3-3z" clip-rule="evenodd"/></svg>
                        </div>
                      </li>
                      <li class="p-4 btn-sidebar cursor-pointer text-xs">
                        <div class="flex items-center justify-center">
                          <svg class="h-4 w-4 text-black"  fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M14.828 14.828a4 4 0 01-5.656 0M9 10h.01M15 10h.01M21 12a9 9 0 11-18 0 9 9 0 0118 0z"/>
                          </svg>
                        </div>
                      </li>
                      <li class="p-4 btn-sidebar cursor-pointer text-xs">GIF</li>
                      <li class="p-4 btn-sidebar cursor-pointer text-xs">STAMP</li>
                      <li class="p-4 btn-sidebar cursor-pointer text-xs">
                        <div class="flex items-center justify-center">
                          <svg class="h-4 w-4 text-black"  viewBox="0 0 24 24" stroke-width="2" stroke="currentColor" fill="none" stroke-linecap="round" stroke-linejoin="round">  <path stroke="none" d="M0 0h24v24H0z"/>  <rect x="4" y="5" width="16" height="16" rx="2" />  <line x1="16" y1="3" x2="16" y2="7" />  <line x1="8" y1="3" x2="8" y2="7" />  <line x1="4" y1="11" x2="20" y2="11" />  <rect x="8" y="15" width="2" height="2" /></svg>
                        </div>
                      </li>
                      <li class="p-4 btn-sidebar cursor-pointer text-xs">...</li>
                      <div class="flex ml-auto">
                        <li class="p-4 btn-sidebar cursor-pointer text-xs">
                          <div>
                            <svg class="h-4 w-4 text-black"  viewBox="0 0 24 24" stroke-width="2" stroke="currentColor" fill="none" stroke-linecap="round" stroke-linejoin="round">  <path stroke="none" d="M0 0h24v24H0z"/>  <line x1="10" y1="14" x2="21" y2="3" />  <path d="M21 3L14.5 21a.55 .55 0 0 1 -1 0L10 14L3 10.5a.55 .55 0 0 1 0 -1L21 3" /></svg>
                          </div>
                        </li>
                      </div>
                    </ul>
                  </div>
                </div>
        </div>
      </div>
    </div>
  </div>
  </div>
</template>

<script>
import MenuBar from '~/components/MenuBar.vue'
import subMenu from '~/components/subMenu.vue'
export default {
  components: {
    MenuBar,
    subMenu
  }
}
</script>
