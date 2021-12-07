<template>
  <div>
    <p>职员：{{ name }}</p>
    <p>年龄：{{ age }}</p>
  </div>
</template>

<script>
export default {
  name: 'School',
  data() {
    return {
      name: '小明',
      age: '18'
    }
  }
}
</script>
