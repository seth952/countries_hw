<template>
  <div id="app">

<h1>Countries</h1>
<div>
  <countries-list :countries='countries'></countries-list>
</div>
  </div>
</template>

<script>
import countriesList from './components/countriesList.vue';

export default {
  name: 'app',
  data(){
    return {
      countries: []
    }
  },
  mounted(){
    fetch('https://restcountries.eu/rest/v2/all')
    .then(response => response.json())
    .then(countries => this.countries = countries)
  },
  components: {
    "countries-list": countriesList
  }
}
</script>

<style>

</style>
