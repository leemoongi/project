<template>
  <div>
    <input
      type="search"
      name=""
      id=""
      @keyup="checkEnter($event)"
      v-model="searchText"
    />
    <button @click="doSearch">조회</button>
  </div>
  <!--
    VUE에서는 kyeup 무슨 키를 눌렀는지 함수처럼 사용가능
    @keyup.enter="doSearch($event)"
    @keyup.ctrl.enter="doSearch()"
   -->
</template>
<script>
export default {
  components: {},
  data() {
    return {
      searchText: ''
    }
  },
  created() {},
  mounted() {},
  unmounted() {},
  methods: {
    doSearch() {
      console.log(this.searchText)
    },
    checkEnter(event) {
      if (event.keyCode === 13) {
        console.log('enter')
      }
    }
  }
}
</script>
