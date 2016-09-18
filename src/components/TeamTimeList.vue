<template>
  <div class="teamtime-list">
    <h1>{{ msg }}</h1>
  </div>
</template>

<script>
export default {
  data: function () {
    console.log('abc')
    if ('geolocation' in navigator) {
      console.log('yes geolocation')
      navigator.geolocation.getCurrentPosition(function (position) {
        console.log(position.coords.latitude, position.coords.longitude)
      })
    } else {
      console.log('oh-no, no geolocation')
    }
    return {
      msg: 'team-time-list'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
