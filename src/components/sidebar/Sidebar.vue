<template>
  <div class="offcanvas-lg offcanvas-start" tabIndex="-1" id="sidebarMenu" aria-labelledby="sidebarMenuLabel">
    <div class="offcanvas-header">
      <p class="offcanvas-title" id="sidebarMenuLabel">gggggggggggg</p>
      <button type="button" class="btn-close" data-bs-dismiss="offcanvas" data-bs-target="#sidebarMenu"
        aria-label="Close"></button>
    </div>
    <div :class="['offcanvas-body d-lg-flex flex-column p-0 pt-4 overflow-y-auto', collapse ? 'text-center' : '']">
      <div class="d-none d-lg-flex justify-content-end ">
        <button @click="toggleCollapse" class="btn btn-sm rounded-circle border ">
          <i :class="collapse ? 'bi bi-arrow-left' : 'bi bi-arrow-right'"></i>
        </button>
      </div>
      <ul v-if="!collapse" class='list-group list-group-flush'>
        <li>a</li>
        <li>a</li>
        <li>a</li>
      </ul>
      <ul v-else class="list-group text-center">
      </ul>
    </div>
  </div>
</template>

<script setup>
defineProps({
  toggleCollapse: {
    type: Function,
    default: false,
  },
  collapse: {
    type: Boolean,
    default: false
  }
})

</script>