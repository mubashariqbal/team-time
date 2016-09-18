<template>
  <div class="app">
    <h1>Team Time</h1>
    <hr>
    <teamtime-list></teamtime-list>
    <hr>
    <set-teamtime></set-teamtime>
  </div>
</template>

<script>
import TeamTimeList from './components/TeamTimeList'
import SetTeamTime from './components/SetTeamTime'

export default {
  components: {
    'teamtime-list': TeamTimeList,
    'set-teamtime': SetTeamTime
  }
}
</script>

<style>
</style>
