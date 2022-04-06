<template>
  <main>
    <SpecialtiesSection/>
    <EventsSection/>
    <LeaderSection/>
    <NewsSection/>
    <TestimonialsSection/>
    <VideoSection/>
    <ContactSection/>
    <!-- <FooterTeach/> -->
  </main>
</template>

<script>
import SpecialtiesSection from './SpecialtiesSection.vue'
import EventsSection from './EventsSection.vue'
import LeaderSection from './LeaderSection.vue'
import NewsSection from './NewsSection.vue'
import TestimonialsSection from './TestimonialsSection.vue'
import VideoSection from './VideoSection.vue'
import ContactSection from './ContactSection.vue'
// import FooterTeach from './FooterTeach.vue'
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
      TestimonialsSection,
      VideoSection,
      ContactSection,
      // FooterTeach,
    }

}
</script>

<style>
    
main{
  margin-bottom: 150px;
}
</style>