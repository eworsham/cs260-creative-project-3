<template>
<div class="events">
  <h1>Schedule</h1>
  <div class="event" v-for="event in events" :key="event.id">
    <h2>{{event.name}}</h2>
    <p>Event Date: {{event.date}}</p>
    <div class="times">
      <p>Start Time: {{event.timeStart}}</p>
      <p>End Time: {{event.timeEnd}}</p>
    </div>
    <p>Number of People Attending: {{event.numberPeople}}</p>
  </div>
</div>
</template>

<script>
export default {
  name: 'eventList',
  props: {
    events: Array
  }
}
</script>

<style>
.event {
  display: flex;
  justify-content: space-around;
  align-items: center;
  margin: .5em 0em;
  border: solid #a1a1a1;
  border-radius: 10px;
}
</style>
