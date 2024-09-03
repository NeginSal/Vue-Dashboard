<template>
  <div class="bg-primary">
    this is sidebar
    <button @click="toggleCollapse" class="btn btn-sm rounded-circle border">
      <i class="bi bi-arrow-left-right fs-5"></i>
    </button>
  </div>
</template>

<script setup>
defineProps({
  toggleCollapse: {
    type: Function,
    default: false,
  },
})

</script>