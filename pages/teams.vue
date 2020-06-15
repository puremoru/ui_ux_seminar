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
                    <span class="text-purple-lightest">Olivia</span>
              </div>

            </div>

            <!-- Chat content -->
            <div class="bg-gray-200 flex flex-col h-screen">
                <!-- Top bar -->
                <div class="border-b flex px-6 py-2 items-center">
                    <div class="flex flex-col">
                        <h3 class="text-grey-darkest text-md mb-1 font-extrabold">#general</h3>
                        <div class="text-grey font-thin text-sm">
                          Chit-chattin' about ugly HTML and mixing of concerns.
                        </div>
                    </div>
                    <div class="ml-auto hidden md:block">
                        <input type="search" placeholder="Search" class="border border-grey rounded-lg p-2"/>
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

                <div class="flex m-15 rounded-lg border-2 border-grey overflow-hidden">
                  <span class="text-3xl text-grey px-3 border-r-2 border-grey">+</span>
                  <input type="text" class="w-full px-4" placeholder="新しいメッセージの入力"/>
                </div>
                <div>
                  <ul class="flex rounded-lg border-2 border-grey overflow-hidden">
                    <li class="p-4 btn-sidebar cursor-pointer text-xs">アイコン</li>
                    <li class="p-4 btn-sidebar cursor-pointer text-xs">アイコン</li>
                    <li class="p-4 btn-sidebar cursor-pointer text-xs">アイコン</li>
                    <li class="p-4 btn-sidebar cursor-pointer text-xs">アイコン</li>
                    <li class="p-4 btn-sidebar cursor-pointer text-xs">アイコン</li>
                    <li class="p-4 btn-sidebar cursor-pointer text-xs">アイコン</li>
                    <li class="p-4 btn-sidebar cursor-pointer text-xs">アイコン</li>
                  </ul>
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
