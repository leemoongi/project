<template>
  <div>
    <div :class="{ 'text-red': hasError, activ: activTrue }">글자입니다</div>
  </div>
</template>
<script>
export default {
  components: {},
  data() {
    return {
      hasError: true,
      activTrue: true
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
