<template>
  <button @click="onClick()" :style="{ background: color }" class="btn">
    {{ text }}
  </button>
  <!-- v-on: click or @ click are the same  -->
</template>

<script>
export default {
  name: "Button",
  props: {
    text: String,
    color: String,
  },
  methods: {
      onClick() {
          console.log('click')
      }
  }
};
</script>
