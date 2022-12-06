<template>
  <div>
    <button @click="addCount">Add {{ counter }}</button>
  </div>
</template>
<script>
export default {
  components: {},
  data() {
    return {
      counter: 0
    }
  },
  created() {},
  mounted() {},
  unmounted() {},
  methods: {
    addCount() {
      this.counter += 1
    }
  }
}
</script>
