<template>
  <div class="container-fluid mx-0 bg-primary">
    <div class="d-flex justify-content-between">
    <a class="navbar-brand" href="#">
      <i class="bi bi-heart-fill d-inline-block align-text-top "></i>
      vuexy
    </a>
    <button @click="toggleCollapse" class="btn btn-sm rounded-circle border">
      <i class="bi bi-arrow-left-right fs-5"></i>
    </button>
  </div>
  </div>

  <!-- <nav class="navbar bg-body-tertiary">
    <div class="container-fluid">
      <a class="navbar-brand" href="#">
        <i class="bi bi-heart-fill d-inline-block align-text-top text-danger"></i>

        Bootstrap
      </a>
    </div>
  </nav> -->
  <!-- <div class="bg-primary">
    this is sidebar
    <button @click="toggleCollapse" class="btn btn-sm rounded-circle border">
      <i class="bi bi-arrow-left-right fs-5"></i>
    </button>
  </div> -->
</template>

<script setup>
defineProps({
  toggleCollapse: {
    type: Function,
    default: false,
  },
})

</script>