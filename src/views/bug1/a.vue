<style scoped>
.content{
  height: 2rem;
  background: #cccccc;
  font-size: 0.4rem;
}
</style>
<template>
  <bug1com>
    <div class="content">我是slot部分 无法触发父级的touchstart事件</div>
  </bug1com>
</template>
<script>
import bug1com from '../../components/bug1com'
export default {
  data () {
    return {
    }
  },
  components: {
    bug1com
  }
}
</script>
