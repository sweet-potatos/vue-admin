<template>
  <div>
    <h1 id="title-dom" ref="title-ref">测试</h1>
    <button id="btn-dom" ref="btn-ref" @click="showDOM">点击事件</button>
    <People id="people-dom" />
    <People ref="people-ref" />
  </div>
</template>

<script>
import People from './components/People.vue'

export default {
  name: 'School',
  components: { People },
  data() {
    return {
      name: '东风南方',
      address: '花都'
    }
  },
  methods: {
    showDOM() {
      const getTitleDom = document.getElementById('title-dom')
      const getTitleRefDom = this.$refs['title-ref']
      console.log('getTitleDom', getTitleDom)
      console.log('getTitleRefDom', getTitleRefDom)

      const getBtnDom = document.getElementById('btn-dom')
      const getBtnRefDom = this.$refs['btn-ref']
      console.log('getBtnDom', getBtnDom)
      console.log('getBtnRefDom', getBtnRefDom)

      const getPeopleDom = document.getElementById('people-dom')
      const getPeopleRefDom = this.$refs['people-ref']
      console.log('getPeopleDom', getPeopleDom)
      console.log('getPeopleRefDom', getPeopleRefDom)
    }
  }
}
</script>
