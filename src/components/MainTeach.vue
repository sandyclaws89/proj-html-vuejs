<template>
  <main>
    <SpecialtiesSection/>
    <EventsSection/>
  </main>
</template>

<script>
import SpecialtiesSection from './SpecialtiesSection.vue'
import EventsSection from './EventsSection.vue'

export default {
    name: 'MainTeach',
    data() {
      return {

      }
    },
    components: {
      SpecialtiesSection,
      EventsSection,
    }

}
</script>

<style lang="scss" scoped>
main{
  margin-bottom: 150px;
}
</style>