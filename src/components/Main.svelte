<script>
  import ChartForSecond from "./ChartForSecond.svelte";
  import ChartForThird from "./ChartForThird.svelte";
  import ChartForThirst from "./ChartForThirst.svelte";
</script>

<div
  class="min-h-screen max-w-[1400px] mx-auto pt-16"
  data-scroll
  data-scroll-section
>
  <div class="flex flex-col">
    <div
      class=" flex flex-col justify-center m-3 gap-3 sm:flex-row sm:flex-wrap"
    >
      <!-- FIRST CARD -->
      <div class="flex flex-col gap-3 sm:w-[310px] xl:w-[300px] z-10">
        <div class="flex flex-col bg-base-200 rounded-lg p-2 sm:p-3">
          <h3 class=" text-xl">Conversions</h3>
          <div class=" text-4xl">200</div>
          <h5>past days 7</h5>
          <ChartForThirst />
        </div>
        <div class="flex flex-col bg-base-200 rounded-lg p-2 gap-4 sm:p-3 pb-6">
          <h5 class=" text-xl">by medium</h5>
          <div>
            <div class="flex justify-between items-center">
              <div>organic</div>
              <div>97</div>
            </div>
            <div class="divider m-0" />
            <div class="flex justify-between items-center">
              <div>organic</div>
              <div>97</div>
            </div>
            <div class="divider m-0" />
            <div class="flex justify-between items-center">
              <div>organic</div>
              <div>97</div>
            </div>
            <div class="divider m-0" />
            <div class="flex justify-between items-center">
              <div>organic</div>
              <div>97</div>
            </div>
            <div class="divider m-0" />
            <div class="flex justify-between items-center">
              <div>organic</div>
              <div>97</div>
            </div>
          </div>
        </div>
      </div>
      <!-- TWO CARD -->
      <div class="flex flex-col gap-3 sm:w-[310px] xl:w-[300px]">
        <div class="flex flex-col bg-base-200 rounded-lg p-2 sm:p-3">
          <h3 class=" text-xl">Conversions</h3>
          <div class=" text-4xl">200</div>
          <h5>past days 7</h5>
          <ChartForSecond />
        </div>
        <div class="flex flex-col bg-base-200 rounded-lg p-2 gap-4 pb-6 sm:p-3">
          <h5 class=" text-xl">by medium</h5>
          <div>
            <div class="flex justify-between items-center">
              <div>organic</div>
              <div>97</div>
            </div>
            <div class="divider m-0" />
            <div class="flex justify-between items-center">
              <div>organic</div>
              <div>97</div>
            </div>
            <div class="divider m-0" />
            <div class="flex justify-between items-center">
              <div>organic</div>
              <div>97</div>
            </div>
            <div class="divider m-0" />
            <div class="flex justify-between items-center">
              <div>organic</div>
              <div>97</div>
            </div>
            <div class="divider m-0" />
            <div class="flex justify-between items-center">
              <div>organic</div>
              <div>97</div>
            </div>
          </div>
        </div>
      </div>
      <!-- THREE CARD -->
      <div class="flex flex-col gap-3 sm:w-[310px] xl:w-[300px]">
        <div class="flex flex-col bg-base-200 rounded-lg p-2 sm:p-3">
          <h3 class=" text-xl">Conversions</h3>
          <div class=" text-4xl">200</div>
          <h5>past days 7</h5>
          <ChartForThird />
        </div>
        <div class="flex flex-col bg-base-200 rounded-lg p-2 gap-4 pb-6 sm:p-3">
          <h5 class=" text-xl">by medium</h5>
          <div>
            <div class="flex justify-between items-center">
              <div>organic</div>
              <div>97</div>
            </div>
            <div class="divider m-0" />
            <div class="flex justify-between items-center">
              <div>organic</div>
              <div>97</div>
            </div>
            <div class="divider m-0" />
            <div class="flex justify-between items-center">
              <div>organic</div>
              <div>97</div>
            </div>
            <div class="divider m-0" />
            <div class="flex justify-between items-center">
              <div>organic</div>
              <div>97</div>
            </div>
            <div class="divider m-0" />
            <div class="flex justify-between items-center">
              <div>organic</div>
              <div>97</div>
            </div>
          </div>
        </div>
      </div>
      <!-- FOUR CARD -->

      <div class="flex flex-col gap-3 sm:w-[310px] xl:w-[300px]">
        <div
          class="bg-base-200 rounded-lg p-2 pb-8 flex flex-col gap-4  sm:p-3"
        >
          <h3 class=" text-xl">Stickinnes - 7 day</h3>
          <div class="flex items-center gap-7">
            <div class="flex flex-col">
              <h1 class="text-4xl">80.03%</h1>
              <h6>New users</h6>
            </div>
            <div class="flex flex-col">
              <h1 class="text-4xl">1.14</h1>
              <h6>Sessions per user</h6>
            </div>
          </div>
        </div>
        <div
          class="bg-base-200 rounded-lg p-2 pb-8 flex flex-col gap-4  sm:p-3"
        >
          <h3 class=" text-xl">Engagement - 7 day</h3>
          <div class="flex items-center gap-7">
            <div class="flex flex-col">
              <h1 class="text-4xl">59<span class=" text-xl">s</span></h1>
              <h6>Avg session...</h6>
            </div>
            <div class="flex flex-col">
              <h1 class="text-4xl">1.47</h1>
              <h6>Pages per session</h6>
            </div>
          </div>
        </div>
        <div
          class="bg-base-200 rounded-lg p-2 pb-8 flex flex-col gap-4  sm:p-3"
        >
          <h3 class=" text-xl">Bounce rate - 7 day</h3>
          <div
            class="radial-progress self-center text-3xl"
            style="--value:70; --size:12rem; --thickness: 20px;"
          >
            70%
          </div>
        </div>
        <div
          class="bg-base-200 rounded-lg p-2 pb-8 flex flex-col gap-4  sm:p-3"
        >
          <h3 class=" text-xl">User locations - LIVE</h3>
          <div class=" self-center">Mape</div>
        </div>
      </div>
    </div>
  </div>
</div>
