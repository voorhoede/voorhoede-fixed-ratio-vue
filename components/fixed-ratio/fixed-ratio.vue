<template>
  <div class="fixed-ratio" :style="{ paddingBottom: `${ratio}%` }">
    <div class="fixed-ratio__content">
      <slot></slot>
    </div>
  </div>
</template>

<script>
  export default {
    props: {
      height: {
        type: Number, 
        required: true
      },
      width: {
        type: Number, 
        required: true
      }
    },
    computed: {
      ratio() {
        return this.height / this.width * 100
      }
    },
}
</script>

<style>
  @import './fixed-ratio.css';
</style>
