<template>
  <div>
    <select>
      <option :value="user.name" :key="user.index" v-for="user in userList">
        {{ user.name }} , {{ user.age }}
      </option>
    </select>
  </div>
</template>
<script>
export default {
  components: {},
  data() {
    return {
      userList: [
        { index: 0, name: '이문기', age: '26' },
        { index: 1, name: '박재성', age: '27' },
        { index: 2, name: '김재범', age: '27' }
      ]
    }
  },
  created() {},
  mounted() {},
  unmounted() {},
  methods: {}
}
</script>
