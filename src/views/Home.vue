<template>
  <div class="list">
    <div @click="jump('bug1')" class="item">
      bug1: click me to view this bug（must ios10-ios11）
    </div>
  </div>
</template>

<script>
export default {
  name: 'home',
  components: {

  },
  methods: {
    jump (name) {
      this.$router.push({ name: name })
    }
  }
}
</script>
<style scoped>
  .list{
    padding: 0.2rem;
  }
  .item{
    height: 0.8rem;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 0.28rem;
    border-bottom: 0.01rem solid #ccc;
  }
</style>
