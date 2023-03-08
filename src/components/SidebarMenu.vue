<template>
  <div class="sidebar"></div>
</template>

<script>
export default {
  name: "SidebarMenu",
};
</script>

<style scoped>
.sidebar {
  width: 100%;
  height: calc(100vh - 75px);
}

@media (max-width: 1100px) {
  .sidebar {
    display: none;
  }
}
</style>
