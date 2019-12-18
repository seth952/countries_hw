<template>
  <div>
    <ul>
      <countries-list v-for="(country, index) in countries" :country="country"
       :key="index"></countries-list>
    </ul>
  </div>
</template>
<script>
export default {
  name: 'countries-list',
  props: ['countries']
}
</script>
<style lang="css" scoped>
</style>
