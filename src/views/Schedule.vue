<template>
<div>
  <eventList :events="events" />
</div>
</template>

<script>
import eventList from "../components/eventList.vue"
export default {
  name: 'Schedule',
  components: {
    eventList
  },
  computed: {
    events() {
      return this.$root.$data.events;
    }
  }
}
</script>
