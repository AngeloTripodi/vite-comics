<script>
import MainHeader from './components/MainHeader.vue';
import ContentSection from './components/ContentSection.vue';
import IconCtaSection from './components/IconCtaSection.vue';
import MainFooter from './components/MainFooter.vue';

export default {
  components: {
    MainHeader,
    ContentSection,
    IconCtaSection,
    MainFooter
  }
}

</script>

<template>
  <MainHeader />
  <ContentSection />
  <IconCtaSection />
  <MainFooter />

</template>

<style lang="scss">
@use './styles/general.scss' as *;
</style>
