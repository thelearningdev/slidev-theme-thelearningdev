<script setup>
import { useSlideContext } from '@slidev/client'
import { computed, ref, useSlots, watchEffect } from 'vue'


const { $clicks } = useSlideContext()
const slots = useSlots()

watchEffect(() => {
  // Track $slidev.nav.clicks reactively
  console.log($clicks.value)
})

const visibleItem = computed(() => {

  const index = $clicks.value - 1
  console.log($clicks, index)
  if (index >= 0 && index < items.value.length) {
    return items.value[index]
  }
  return null
})
</script>

<template>
  <div>
    <component :is="visibleItem" v-if="visibleItem" />
  </div>
</template>
