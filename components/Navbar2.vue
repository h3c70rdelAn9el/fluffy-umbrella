<template>
  <b-navbar class="navbar" toggleable="md" type="light">
    <b-navbar-brand href="#">
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
        <b-nav-item href="#">
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
    background: rgb(209, 101, 209);
  }

  .nav-icon {
    color: black;
  }
</style>
