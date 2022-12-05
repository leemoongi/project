<template>
  <div>
    <div style="color: red; font-size: 30px">1.글씨는 red, 폰트 30px</div>
    <div :style="styleObj">2.글씨는 red, 폰트 30px</div>
    <button @click="changColor">색 변경</button>
  </div>
</template>
<script>
export default {
  components: {},
  data() {
    return {
      styleObj: { color: 'green', fontSize: '30px' }
    }
  },
  created() {},
  mounted() {},
  unmounted() {},
  methods: {
    changColor() {
      this.styleObj.color = 'darkorchid'
    }
  }
}
</script>
