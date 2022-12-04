<template>
  <TheHeader></TheHeader>
  <Content></Content>
  <Banner1></Banner1>
  <TheFooter></TheFooter>
  <Banner2></Banner2>
</template>
<script >
import TheHeader from './components/TheHeader.vue';
import Content from './components/Content.vue';
import Banner1 from './components/Banner1.vue';
import TheFooter from './components/TheFooter.vue';
import Banner2 from './components/Banner2.vue';
export default{
  components: {TheHeader, Content, Banner1, TheFooter, Banner2}

}

</script>


<style lang="scss">
@use "./styles/general.scss"

</style>
