<template>
  <main>
    <SpecialtiesSection/>
    <EventsSection/>
    <LeaderSection/>
  </main>
</template>

<script>
import SpecialtiesSection from './SpecialtiesSection.vue'
import EventsSection from './EventsSection.vue'
import LeaderSection from './LeaderSection.vue'

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
    }

}
</script>

<style lang="scss" scoped>
main{
  margin-bottom: 150px;
}
</style>