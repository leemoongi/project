<template>
  <div>
    <input type="text" v-bind:value="userId" readonly />
    <input type="text" :value="userId" readonly />
    <button @click="condoleLog">로그</button>
    <br />
    <br />
    <img :src="imgSrc" style="width: 300px; height: auto" />
    <input type="search" v-model="searchTxt" />
    <button :disabled="searchTxt === ''">조회</button>
  </div>
</template>
<script>
export default {
  components: {},
  data() {
    return {
      userId: 'MoonGi',
      imgSrc:
        'https://petcebook.com/data/ko-KR/modoo/2022-04/3ba2b25dcbe48bbb0d831e91ac34d7fd.png',
      searchTxt: ''
    }
  },
  created() {},
  mounted() {},
  unmounted() {},
  methods: {
    condoleLog() {
      console.log(this.userId)
    }
  }
}
</script>
