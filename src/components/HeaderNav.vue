<template>
  <header>
    <b-navbar toggleable="lg" type="light" variant="light" class="p-3">
      <b-navbar-brand href="#">PeakU</b-navbar-brand>

      <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

      <b-collapse id="nav-collapse" is-nav class="justify-content-end">
        <b-navbar-nav>
          <b-nav-item active href="#">Jobs</b-nav-item>
          <b-nav-item href="#">Bootcamp</b-nav-item>
          <b-nav-item href="#">About Us</b-nav-item>
        </b-navbar-nav>

        <!-- Right aligned nav items -->
        <b-navbar-nav class="ml-auto">
          <b-nav-item-dropdown text="For professionals" right>
            <b-dropdown-item href="#">Home</b-dropdown-item>
            <b-dropdown-item href="#">Jobs</b-dropdown-item>
            <b-dropdown-item href="#">Courses and challenges</b-dropdown-item>
            <b-dropdown-item href="#">Questions</b-dropdown-item>
            <b-dropdown-item href="#">Teachers</b-dropdown-item>
            <b-dropdown-item href="#">Bootcamp</b-dropdown-item>
          </b-nav-item-dropdown>

          <b-nav-item-dropdown text="For business" right class="me-2">
            <b-dropdown-item href="#">Home</b-dropdown-item>
            <b-dropdown-item href="#">Our process</b-dropdown-item>
            <b-dropdown-item href="#">Plans</b-dropdown-item>
            <b-dropdown-item href="#">Assessments</b-dropdown-item>
            <b-dropdown-item href="#">Payroll</b-dropdown-item>
            <b-dropdown-item href="#">Blog</b-dropdown-item>
            <b-dropdown-item href="#">Sales</b-dropdown-item>
            <b-dropdown-item href="#">Calculator</b-dropdown-item>
          </b-nav-item-dropdown>
        </b-navbar-nav>

        <b-navbar-nav>
          <b-nav-item href="#">English</b-nav-item>
          <b-nav-item href="#" style="border: 1px solid #dee2e6; padding: 0 5px"
            ><i class="fa-sharp fa-solid fa-bell"></i
          ></b-nav-item>
          <b-nav-item
            href="#"
            class="ms-2"
            style="border: 1px solid #dee2e6; padding: 0 5px"
            ><i class="fa-solid fa-user"></i
          ></b-nav-item>
        </b-navbar-nav>
      </b-collapse>
    </b-navbar>
  </header>
</template>

<script>
export default {
  name: "HeaderNav",
};
</script>

<style scoped></style>
