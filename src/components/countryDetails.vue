<template>
  <div v-if='country'>
    <p>Capital: {{country.capital}}</p>
    <p>Region: {{country.region}}</p>
    <p>Population: {{country.population}}</p>
    

  </div>
</template>
<script>

export default {
  name: "country-details",
  props: ['country']
}
</script>
<style lang="css" scoped>
</style>
