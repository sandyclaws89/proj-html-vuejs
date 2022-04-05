<template>
  <main>
    <SpecialtiesSection/>
    <EventsSection/>
    <LeaderSection/>
    <NewsSection/>
  </main>
</template>

<script>
import SpecialtiesSection from './SpecialtiesSection.vue'
import EventsSection from './EventsSection.vue'
import LeaderSection from './LeaderSection.vue'
import NewsSection from './NewsSection.vue'

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
      NewsSection
    }

}
</script>

<style lang="scss" scoped>
main{
  margin-bottom: 150px;
}
</style>