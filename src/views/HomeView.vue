<template>
  <div class="container-fluid">
    <div class="row">
      <div :class="['bg-primary', collapse ? 'col-lg-1' : 'col-lg-2']">
        <Sidebar :toggleCollapse="toggleCollapse" :collapse="collapse" />
      </div>
      <div :class="['bg-danger', collapse ? 'col-lg-11' : 'col-lg-10']">dddddddd</div>
    </div>
  </div>
</template>

<script setup>
import Sidebar from '@/components/sidebar/Sidebar.vue';
import { ref } from 'vue'
const collapse = ref(false);

const toggleCollapse = () => {
  collapse.value = !collapse.value;
};

</script>
