<template>
  <svg
    :width="width"
    :height="height"
    :viewBox="`0 0 ${width} ${height}`">
    <rect
      :class="color"
      x="0"
      y="0"
      :width="width"
      :height="height"
      rx="8"
      ry="8"
    ></rect>
    <text
      :x="width / 2"
      y="30"
      fill="#000000"
      text-anchor="middle"
      font-size="20px"
    >{{ text }}</text>
  </svg>
</template>

<script>
export default {
  name: 'svgRect',

  props: {
    text: {
      type: String,
      required: true,
    },
    width: {
      type: Number,
    },
    height: {
      type: Number,
      required: true,
    },
    color: {
      type: String,
      required: true,
    }
  },

  // data() {
  //   return {
  //     color: 'yellow'
  //   }
  // }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="sass">
.green
  fill: #31c978
.red
  fill: #ffa5ab
.yellow
  fill: #ffec70
</style>
