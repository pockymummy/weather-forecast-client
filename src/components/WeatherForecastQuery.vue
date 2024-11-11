<script setup>
const lat = 0.00;
const lon = 0.00;
const forecastDate = Date.now();
const hour = 0;
</script>

<template>
  <div class="weather-forecast-query">
    <form class="weather-forecast-query-form" @submit.prevent="">
        <div class="weather-forecast-query-form-input-fields">
            <label for="lat">Lat:</label>
            <input id="lat" v-model.number="lat">
            <label for="lon">Lon:</label>
            <input id="lon" v-model.number="lon">
            <label for="forecastDate">Date:</label>
            <input type="date" id="forecastDate" name="forecastDate" v-model="forecastDate" />
            <label for="hour">Hour:</label>
            <input id="hour" v-model.number="hour">
        </div>
        <input class="button" type="submit" value="Query">
    </form>
  </div>
</template>

<style scoped>

</style>
