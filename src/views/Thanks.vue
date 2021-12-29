<template>
  <div>
    <div class="h-full w-full flex items-center justify-center">
      <h1
        class="text-2xl font-boldHeadline uppercase text-secondary dark:text-primary"
      >
        Thanks for contacting us, we'll be in touch soon.
      </h1>
    </div>
    <Footer class="bg-primary dark:bg-secondary" />
  </div>
</template>

<script>
import Footer from '../components/Footer.vue';

// @ is an alias to /src

export default {
  name: 'ComingSoon',
  components: {
    Footer,
  },
  data() {
    return {};
  },

  watch() {},
};
</script>

<style></style>
