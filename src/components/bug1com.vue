<style>
  .box{
    padding: 0.2rem 0.2rem 2rem;
    background: #42b983;
    font-size: 0.4rem;
  }
</style>
<template>
  <div class="box" @touchstart="onTouchStart">
    i am parent, i bind a touchstart event

    <slot></slot>
  </div>
</template>
<script>
export default {
  data () {
    return {
      txt: ''
    }
  },
  methods: {
    onTouchStart (e) {
      this.txt = new Date().getTime()
    }
  }
}
</script>
