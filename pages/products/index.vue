<template>
  <div>
    <div class="container">
      <LargeCardDisplay
        v-for="cardInfo in largeCardInfo"
        :key="cardInfo"
        :cards-section="cardInfo"
      />
      <SmallCardDisplay
        v-for="cardInfo in smallCardInfo"
        :key="cardInfo"
        :cards-section="cardInfo"
      />
    </div>
  </div>
</template>

<script>
import { largeCardSections, smallCardSections } from '@/assets/data'

export default {
  data () {
    return {
      largeCardInfo: largeCardSections,
      smallCardInfo: smallCardSections
    }
  }
}
</script>

<style scoped></style>
