<template>
  <div>
    <HeaderNav />
    <div class="row">
      <div class="aside col-md-1">
        <SidebarMenu />
      </div>
      <div class="content col-md-11">
        <SearchBar />
        <CardContainer />
      </div>
    </div>
  </div>
</template>

<script>
import HeaderNav from "./components/HeaderNav.vue";
import SearchBar from "./components/SearchBar.vue";
import SidebarMenu from "./components/SidebarMenu.vue";
import CardContainer from "./components/CardContainer.vue";

export default {
  name: "App",
  components: {
    HeaderNav,
    SidebarMenu,
    SearchBar,
    CardContainer,
  },
};
</script>

<style>
body {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  overflow-x: hidden;
  background-color: #f8f9fa !important;
}

@media screen and (max-width: 1100px) {
  .aside {
    display: none;
  }

  .content {
    width: 100% !important;
  }
}
</style>
