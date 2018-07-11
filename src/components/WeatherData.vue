<template>
    <dl>
        <dt v-if="weatherData.temp != weatherData.temp_min">Current Temp</dt>
        <dd v-if="weatherData.temp != weatherData.temp_min">{{ weatherData.temp }}&deg;C</dd>
        <dt>Humidity</dt>
        <dd>{{ weatherData.humidity }}%</dd>
        <dt>High</dt>
        <dd>{{ weatherData.temp_max }}&deg;C</dd>
        <dt>Low</dt>
        <dd>{{ weatherData.temp_min }}&deg;C</dd>
    </dl>
</template>

<script>
export default {
  name: 'WeatherData',
  data () {
    return {

    }
  },
  props: {
    weatherData: Object
  }
}
</script>

<style scoped>
dl {
  padding: 5px;
  color: #000000;
  background: #d0e6e9;
}
dt {
  float: left;
  clear: left;
  width: 120px;
  text-align: right;
  font-weight: bold;
  color: #3e4a58;
}
dd {
  margin: 0 0 0 130px;
  padding: 0 0 0.5em 0;
}
dt::after {
  content: ":";
}
</style>