<template>
  <div class="events">
    <h1>Event For Good</h1>
    <EventCard  v-for="event in events" :key="event.id" :event='event' />

  </div>
</template>

<script>
// @ is an alias to /src
import EventCard from "@/components/EventCard.vue";

export default {
  name: "EventList",
  components: {
    EventCard,
  },

   data () {
    return {
      events : [ 

       { 
         id : 5555555,
        category : 'animal welfare',
        title : 'Cat abdotion Day',
        description : 'Find your new feline friend at this event',
        location : 'yangon',
        date : 'january 28, 2022',
        time : '12:00',
        petsAllowed : true,
        origanizer  : 'Zaw Naing Oo'
        },
        { 
         id : 8888888,
        category : 'animal welfare',
        title : 'Rabbit abdotion Day',
        description : 'Find your new feline friend at this event',
        location : 'yangon',
        date : 'january 28, 2022',
        time : '12:00',
        petsAllowed : true,
        origanizer  : 'Zaw Naing Oo'
        },
        { 
         id : 9999999,
        category : 'animal welfare',
        title : 'Dog abdotion Day',
        description : 'Find your new feline friend at this event',
        location : 'yangon',
        date : 'january 28, 2022',
        time : '12:00',
        petsAllowed : true,
        origanizer  : 'Zaw Naing Oo'
        }

       ]
    }
 }


};
</script>

<style scoped>

.events{
  display: flex;
  flex-direction: column;
  align-items: center;
}
</style>
