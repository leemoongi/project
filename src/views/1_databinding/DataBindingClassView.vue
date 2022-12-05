<template>
  <div>
    <div :class="{ 'text-red': ture, activ: ture }"></div>
  </div>
</template>
<script>
export default {
  components: {},
  data() {
    return {
      sampleData: ''
    }
  },
  created() {},
  mounted() {},
  unmounted() {},
  methods: {}
}
</script>

<style scoped>
.activ {
  background-color: aqua;
  font-weight: bold;
}
.text-red {
  color: red;
}
</style>
