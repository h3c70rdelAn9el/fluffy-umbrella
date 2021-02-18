<template>
  <b-navbar class="navbar" toggleable="md" type="light">
    <b-navbar-brand href="#" class="brand">
      brand
    </b-navbar-brand>
    <b-navbar-toggle target="navbar-toggle-collapse">
      <template v-slot:default="{ expanded }">
        <b-icon v-if="expanded" class="nav-icon" icon="chevron-bar-up" />
        <b-icon v-else icon="chevron-bar-down" class="nav-icon" />
      </template>
    </b-navbar-toggle>
    <b-collapse id="navbar-toggle-collapse" is-nav>
      <b-navbar-nav class="ml-auto">
        <b-nav-item href="#" class="nav-links">
          foo
        </b-nav-item>
        <b-nav-item href="#">
          bar
        </b-nav-item>
      </b-navbar-nav>
    </b-collapse>
  </b-navbar>
</template>

<style scoped>
  .navbar {
    background: rgb(111, 45, 155);
  }
  .nav-icon {
    color: black;
  }

 .navbar a:hover {
    background-color: rgb(163, 133, 184);
    border-radius: 5px;
  }

  .navbar a {
    padding-left: 2px;
  }
</style>
