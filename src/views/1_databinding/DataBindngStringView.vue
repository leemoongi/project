<template>
  <div>
    <h1>Hello {{ userName }}</h1>
    <p>{{ message }}</p>
  </div>
</template>

<script>
export default {
  data() {
    return {
      userName: 'Moon Gi',
      message: 'vue 마스터 가즈아~!!',
      arr: [],
      obj: {}
    }
  }
}
</script>
<style scoped>
.text-read {
  color: red;
}
</style>
