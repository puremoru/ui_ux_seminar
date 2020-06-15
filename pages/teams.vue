<template>
  <div>
    <MenuBar />
    <div class="inline-block absolute ">
      <div class="w-full border shadow h-screen">
	      <div class="flex">
            <!-- Sidebar / channel list -->
            <div class="text-purple-lighter w-1/4 pb-6 hidden md:block">
                <div class="flex items-center mb-6 px-4">
                  <span class="bg-green rounded-full block w-2 h-2 mr-2"></span>
                    <span class="text-purple-lightest">チャット</span>
              </div>

            </div>

            <!-- Chat content -->
            <div class="bg-gray-200 flex flex-col h-screen">
                <!-- Top bar -->
                <div class="border-b flex px-6 py-2 items-center">
                    <div class="flex">
                        <h3 class="text-grey-darkest text-lg mb-1 font-extrabold flex-initial px-1">hogehoge</h3>
                        <h3 class="text-grey-darkest text-base mb-1 flex-initial px-1">Chat</h3>
                        <h3 class="text-grey-darkest text-base mb-1 flex-initial px-1">Files</h3>
                        <h3 class="text-grey-darkest text-base mb-1 flex-initial px-1">Organization</h3>
                        <h3 class="text-grey-darkest text-base mb-1 flex-initial px-1">Activity</h3>
                        <h3 class="text-grey-darkest text-base mb-1 flex-initial px-1">+</h3>
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
                        <img src="https://avatars2.githubusercontent.com/u/343407?s=460&v=4" class="w-10 h-10 rounded mr-3" />
                        <div class="flex flex-col">
                            <div class="flex items-end">
                              <span class="font-bold text-md mr-2 font-sans">killgt</span>
                              <span class="text-grey text-xs font-light">11:46</span>
                            </div>
                          <p class="font-light text-md text-grey-darkest pt-1">The slack from the other side.</p>
                        </div>
                    </div>

                    <!-- A message -->
                    <div class="flex items-start mb-4">
                        <img src="https://i.imgur.com/8Km9tLL.jpg" class="w-10 h-10 rounded mr-3" />
                        <div class="flex flex-col">
                            <div class="flex items-end">
                              <span class="font-bold text-md mr-2 font-sans">Olivia Dunham</span>
                              <span class="text-grey text-xs font-light">12:45</span>
                            </div>
                          <p class="font-light text-md text-grey-darkest pt-1">How are we supposed to control the marquee space without an utility for it? I propose this:</p>
                            <div class="bg-grey-lighter border border-grey-light font-mono rounded p-3 mt-2 whitespace-pre">.marquee-lightspeed { -webkit-marquee-speed: fast; }
    .marquee-lightspeeder { -webkit-marquee-speed: faster; }</div>
                        </div>
                    </div>

                    <!-- A message -->
                    <div class="flex items-start">
                        <img src="https://i.imgur.com/qACoKgY.jpg" class="w-10 h-10 rounded mr-3" />
                        <div class="flex flex-col">
                            <div class="flex items-end">
                              <span class="font-bold text-md mr-2 font-sans">Adam Bishop</span>
                              <span class="text-grey text-xs font-light">12:46</span>
                            </div>
                          <p class="font-light text-md text-grey-darkest pt-1"><a href="#" class="text-blue">@Olivia Dunham</a> the size of the generated CSS is creating a singularity in space/time, we must stop adding more utilities before it's too late!</p>
                        </div>
                    </div>

                </div>

                <div class="flex m-16 rounded-lg border-2 border-grey overflow-hidden">
                  <span class="text-3xl text-grey px-3 border-r-2 border-grey">+</span>
                  <input type="text" class="w-full px-4" placeholder="新しいメッセージの入力"/>
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
