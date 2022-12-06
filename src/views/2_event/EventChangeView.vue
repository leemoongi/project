<template>
  <div>
    <select @change="changCity" v-model="selectedCity">
      <option value="000">==도시 선택==</option>
      <option
        :value="city.cityCode"
        :key="city.cityCode"
        v-for="city in cityList"
      >
        {{ city.name }}
      </option>
    </select>
    <select>
      <option :key="dong.dongCode" v-for="dong in selectedDongList">
        {{ dong.name }}
      </option>
    </select>
    <select>
      <option
        :key="dong.dongCode"
        v-for="dong in dongList.filter(
          (dong) => dong.cityCode === this.selectedCity
        )"
      >
        {{ dong.name }}
      </option>
    </select>
  </div>
</template>
<script>
export default {
  components: {},
  data() {
    return {
      cityList: [
        { cityCode: '100', name: '서울' },
        { cityCode: '200', name: '부산' },
        { cityCode: '300', name: '대구' },
        { cityCode: '400', name: '대전' },
        { cityCode: '500', name: '영천' }
      ],
      dongList: [
        { cityCode: '100', dongCode: '1', name: '서울1동' },
        { cityCode: '100', dongCode: '2', name: '서울2동' },
        { cityCode: '100', dongCode: '3', name: '서울3동' },
        { cityCode: '200', dongCode: '4', name: '부산1동' },
        { cityCode: '200', dongCode: '5', name: '부산1동' },
        { cityCode: '300', dongCode: '6', name: '대구1동' },
        { cityCode: '400', dongCode: '7', name: '대전1동' },
        { cityCode: '500', dongCode: '8', name: '영천1동' }
      ],
      selectedCity: '000',
      selectedDongList: []
    }
  },
  created() {},
  mounted() {},
  unmounted() {},
  methods: {
    changCity() {
      this.selectedDongList = this.dongList.filter(
        (dong) => dong.cityCode === this.selectedCity
      )
    }
  }
}
</script>
