<template>
  <div>
    <div>{{ htmlString }}</div>
    <div v-html="htmlString"></div>
  </div>
</template>
<script>
export default {
  components: {},
  data() {
    return {
      htmlString: '<p style="color:red">빨간문자</p>'
    }
  },
  created() {},
  mounted() {},
  unmounted() {},
  methods: {}
}
</script>
