<template>
  <div>
    <div
      class="flex flex-col lg:grid lg:grid-cols-2 lg:grid-rows-2 items-center p-2 md:p-10"
    >
      <div class="flex justify-center">
        <div
          class="w-82 2xl:w-full flex px-auto items-center justify-center flex-col text-center m-10 dark:text-primary"
        >
          <h1 class="font-boldHeadline text-2xl w-full">LIVE Standings</h1>
          <p class="font-headline text-sm dark:text-gray-500 mt-5">
            Stay up to date with the latest driver and constructor standings in
            the current championship battles.
          </p>

          <div class="flex flex-col">
            <a
              class="flex items-start"
              href="https://apps.apple.com/gb/app/formula-gp-2k/id1602496701"
              target="_blank"
            >
              <button
                class="m-10 flex w-52 text-white bg-purple border-0 py-2 px-4 focus:outline-none items-center text-left hover:bg-red-700 rounded text-xs font-headline"
              >
                <div class="h-full">
                  <i class="fab fa-apple text-3xl px-2.5"></i>
                </div>
                <div class="flex flex-col w-2/3">
                  <p class="">Download on the</p>
                  <p class="text-lg font-bold">App Store</p>
                </div>
              </button>
            </a>
          </div>
        </div>
      </div>
      <div>
        <div class="mockup-phone border-primary">
          <div class="camera"></div>
          <div class="display">
            <div class="artboard phone-1 artboard-demo bg-light dark:bg-dark">
              <img
                class="w-full object-cover pt-28"
                src="../assets/screenshot7.png"
                alt=""
              />
            </div>
          </div>
        </div>
      </div>
      <!--  -->
      <div
        class="flex lg:hidden w-82 2xl:w-full px-auto items-center justify-center flex-col text-center m-10 dark:text-primary"
      >
        <h1 class="font-boldHeadline text-2xl w-full">Head to Head</h1>
        <p class="font-headline text-sm dark:text-gray-500 mt-5">
          Check out how the drivers stack up against one another within each
          team,
          <span>compare their stats too see who is coming out on top!</span>
        </p>

        <div class="flex flex-col"></div>
      </div>

      <div class="m-10">
        <div class="mockup-phone border-primary">
          <div class="camera"></div>
          <div class="display">
            <div class="artboard phone-1 artboard-demo bg-light dark:bg-dark">
              <img class="dark" src="../assets/screenshot.png" alt="" />
            </div>
          </div>
        </div>
      </div>
      <div
        class="hidden lg:flex w-82 2xl:w-full px-auto items-center justify-center flex-col text-center m-10 dark:text-primary"
      >
        <h1 class="font-boldHeadline text-2xl w-full">Head to Head</h1>
        <p class="font-headline text-sm dark:text-gray-500 mt-5">
          Check out how the drivers stack up against one another within each
          team,
          <span>compare their stats too see who is coming out on top!</span>
        </p>

        <div class="flex flex-col"></div>
      </div>
    </div>
    <div></div>

    <Footer class="bg-primary dark:bg-secondary" />
  </div>
</template>

<script>
import Footer from '../components/Footer.vue';
import { mapGetters } from 'vuex';
// @ is an alias to /src

export default {
  name: 'Home',
  data() {
    return {
      toggleDarkModeFalse: false,
    };
  },
  components: { Footer },
  watch() {
    this.$store.state.darkMode;
  },
  computed: {
    ...mapGetters(['toggleDarkModeFalse', 'toggleDarkModeTrue']),
  },
};
</script>

<style scoped>
/* button:hover p {
  display: none;
}

button:hover:before {
  content: 'Coming Soon!';
  height: 45px;
  display: flex;
  justify-content: center;
  place-items: center;
  padding: 10px;
  font-size: 20px;
  text-decoration: underline;
  line-height: 20px;
} */
</style>
