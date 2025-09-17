<template>
  <div class="slidev-layout cover">
    <div class="my-auto w-full text-center">
      <slot />
    </div>
  </div>
</template>

<script setup>
defineProps({
  number: {
    type: String,
    default: ''
  }
})
</script>

