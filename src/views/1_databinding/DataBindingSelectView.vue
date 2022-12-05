<template>
  <div>
    <select v-model="selectedCity">
      <option value=""></option>
      <option value="02">서울</option>
      <option value="051">부산</option>
      <option value="064">제주</option>
    </select>
    <br />
    <button @click="condoleLog">로그보기</button>
  </div>
</template>
<script>
export default {
  components: {},
  data() {
    return {
      selectedCity: '051'
    }
  },
  created() {},
  mounted() {},
  unmounted() {},
  methods: {
    condoleLog() {
      console.log(this.selectedCity)
    }
  }
}
</script>
