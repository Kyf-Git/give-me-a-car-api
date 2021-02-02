<template>

<div class="body"><Sidebar class="sidebar"/><FullStockAgence class="tableau" /></div>

</template>


<style>

</style>


<script>
export default {
  components: { FullStockAgence , Sidebar},
  name: "Dashboard",
  

};

import FullStockAgence from '../components/Tables/FullStockAgence.vue';
import Sidebar from '../components/SideBarPlugin/SideBar'
</script>

