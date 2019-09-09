<template>
  <div v-if="loading" class="loading">
    疯狂加载中...
    <img :src="url" alt="" />
  </div>
</template>

<script>
export default {
  data() {
    return {
      loading: false,
      url: 'http://pwtrnh84p.bkt.clouddn.com//blog/%E6%B5%A6%E4%B8%9C%E6%96%B0%E5%8C%BA-%E5%BC%A0%E6%B1%9F%E9%AB%98%E7%A7%91-%E5%8D%8E%E8%99%B9%E7%A7%91%E6%8A%80%E5%9B%ADC%E5%8C%BA.jpeg'
    }
  },
  methods: {
    start() {
      this.loading = true
    },
    finish() {
      this.loading = true
    }
  }
}
</script>
<style lang="less" scoped>
.loading {
  position: fixed;
  top: 50%;
  left: 50%;
  transform: translateX(-50%) translateY(-50%);
  color: #000;
  font-size: 22px;
  img {
    width: 50px;
    height: 50px;
  }
}
</style>
