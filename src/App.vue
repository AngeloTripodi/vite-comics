<script>
import MainHeader from './components/MainHeader.vue';
import MainJumbo from './components/MainJumbo.vue';
import ContentSection from './components/ContentSection.vue';
import IconCtaSection from './components/IconCtaSection.vue';
import MainFooter from './components/MainFooter.vue';


export default {
  components: {
    MainHeader,
    MainJumbo,
    ContentSection,
    IconCtaSection,
    MainFooter
  }
}

</script>

<template>
  <MainHeader />
  <main>
    <MainJumbo />
    <ContentSection />
    <IconCtaSection />
  </main>
  <MainFooter />

</template>

<style lang="scss">
@use './styles/general.scss' as *;
</style>
