<template>
  <main role="main">
    <h1>Fixed Ratio</h1>
    
    <p>ratio 16/9, real dimensions image: 800x600</p>
    <fixed-ratio :width="16" :height="9">
      <img src="https://picsum.photos/800/600/" alt="">
    </fixed-ratio>

    <p>ratio 2/1, real dimensions image: 900x400</p>
    <fixed-ratio :width="2" :height="1">
      <img src="https://picsum.photos/900/400/" alt="">
    </fixed-ratio>

    <p>ratio 1/1, real dimensions image: 900x700</p>
    <fixed-ratio :width="1" :height="1">
      <img src="https://picsum.photos/900/700/" alt="">
    </fixed-ratio>

    <p>ratio 2/1, real dimensions image: 400x200</p>
    <fixed-ratio :width="2" :height="1">
      <img src="https://picsum.photos/400/200/" alt="">
    </fixed-ratio>
  </main>
</template>

<script>
  import FixedRatio from '../components/fixed-ratio/fixed-ratio'

  export default {
    components: { FixedRatio }
  }
</script>

<style>
  [role="main"] {
    margin-left: auto;
    margin-right: auto;
    max-width: 600px;
  }
</style>
