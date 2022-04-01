<template>
  <main>
    <SpecialtiesSection/>
  </main>
</template>

<script>
import SpecialtiesSection from './SpecialtiesSection.vue'

export default {
    name: 'MainTeach',
    data() {
      return {

      }
    },
    components: {
      SpecialtiesSection
    }

}
</script>

<style>
main{
  margin-bottom: 150px;
}
</style>