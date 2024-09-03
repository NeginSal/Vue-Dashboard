<script setup>
import Sidebar from '@/components/sidebar/Sidebar.vue';
import { ref } from 'vue'
const collapse = ref(false);

const toggleCollapse = () => {
  collapse.value = !collapse.value;
};
</script>

<template>
  <div class="container-fluid">
    <div class="row">
      <div :class="collapse ? 'col-lg-1' : 'col-lg-2' ">
        <Sidebar :toggleCollapse="toggleCollapse"/>
      </div>
      <div class="col-lg-10 bg-danger">dddddddd</div>
    </div>
  </div>
</template>
