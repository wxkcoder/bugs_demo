<style scoped>
.content{
  height: 2rem;
  background: #cccccc;
  font-size: 0.4rem;
}
</style>
<template>
  <bug1com>
    <div class="content">i am slot content , i can't trigger parent's touchstart event</div>
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
