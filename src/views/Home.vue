<template>
  <div class="home">
    <svgRect width="200" height="50" text="VueJS" color="yellow"/>
    <svgRect width="200" height="50" text="VueJS" color="green"/>
    <svgRect width="200" height="50" text="VueJS" color="red"/>
  </div>
</template>

<script>
// @ is an alias to /src
import svgRect from "@/components/svgRect.vue";

export default {
  name: "Home",

  components: {
    svgRect,
  },
};
</script>
