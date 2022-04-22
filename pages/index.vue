<template>
  <div>
    <NavBar />
    <div class="container">
      <HeroView />
      <LargeCardDisplay
        v-for="cardInfo in largeCardInfo"
        :key="cardInfo.id"
        :card-section="cardInfo"
      />
      <SmallCardDisplay
        v-for="cardInfo in smallCardSections"
        :key="cardInfo.id"
        :card-section="cardInfo"
      />
    </div>
  </div>
</template>

<script>
// import HeroView from '../components/HeroView.vue'
// import LargeCardDisplay from '../components/LargeCardDisplay.vue'
// import SmallCardDisplay from '../components/SmallCardDisplay.vue'
import { largeCardSections, smallCardSections } from '@/assets/data.js'
export default {
  name: 'IndexPage',
  // components: {
  //   HeroView,
  //   LargeCardDisplay,
  //   SmallCardDisplay,
  // },
  data() {
    return {
      largeCardInfo: largeCardSections,
      smallCardSections,
    }
  },
}
</script>
