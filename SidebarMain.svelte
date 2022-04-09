<script>
  import SidebarFooter from "./SidebarFooter.svelte";
</script>

<style>
  /* iframe a {
                                                                                                                                                                                                                                                                                                                                                                                                        display: none;
                                                                                                                                                                                                                                                                                                                                                                                                      } */
</style>

<aside class="w-96">
  <div class="lg:w-80 lg:h-screen h-1/2 py-16 px-4 static lg:fixed flex flex-col justify-between">
      <!-- header -->
      <div class="">
        <h1 class="text-5xl font-extrabold w-full lg:h-[288px] h-[235px] focus:outline-0 lg:text-left text-center whitespace-normal">
          
          <div class="text-lg font-bold relative top-36 z-10">The Online</div>
          <strong class="relative top-36 z-10">Passion Reader</strong>
          <iframe title="logo" class="absolute top-4 z-0 h-[400px]" src='https://my.spline.design/passionreader-2dd17c69f8d352d9e0df43e7f915a6c5/' frameborder='0'></iframe>

        </h1>
       
        <p class="z-10 relative font-semibold text-slate-400 lg:mt-0 mt-10 lg:text-left text-center whitespace-normal">
          Articles to help you meditate on the events of Jesus' final week.
        </p>
        
      </div>
      
      <!-- changed div class to remove footer (on top) from DOM when mobile-->
      <div class="lg:block hidden">
        <SidebarFooter />
      </div>
      
  </div>

</aside>