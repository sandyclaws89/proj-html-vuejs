<template>
  <main>
    <SpecialtiesSection/>
    <EventsSection/>
    <LeaderSection/>
    <NewsSection/>
    <TestimonialsSection/>
  </main>
</template>

<script>
import SpecialtiesSection from './SpecialtiesSection.vue'
import EventsSection from './EventsSection.vue'
import LeaderSection from './LeaderSection.vue'
import NewsSection from './NewsSection.vue'
import TestimonialsSection from './TestimonialsSection.vue'

export default {
    name: 'MainTeach',
    data() {
      return {

      }
    },
    components: {
      SpecialtiesSection,
      EventsSection,
      LeaderSection,
      NewsSection,
      TestimonialsSection
    }

}
</script>

<style>
    
main{
  margin-bottom: 150px;
}
</style>