<style>
  .box{
    padding: 0.2rem 0.2rem 2rem;
    background: #42b983;
    font-size: 0.4rem;
  }
</style>
<template>
  <div class="box" @touchstart="onTouchStart">
    我是组件盒子部分 绑定了touchstart事件 触发时间：{{txt}}

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
