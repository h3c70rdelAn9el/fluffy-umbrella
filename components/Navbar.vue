<template>
  <b-navbar toggleable="md" type="dark" variant="dark">
    <b-navbar-brand href="#">
      Logo
    </b-navbar-brand>
    <b-navbar-nav class="ml-auto">
      <b-nav-item-dropdown text="" class="navbar-dropdown" right>
        <template v-slot:button-content>
          <span>Menu</span>
        </template>
        <b-dropdown-item href="#">
          link A
        </b-dropdown-item>
        <b-dropdown-item href="#">
          link B
        </b-dropdown-item>
      </b-nav-item-dropdown>
    </b-navbar-nav>
  </b-navbar>
</template>

<style>
  .navbar-dropdown {
    background-color: black;
  }
</style>
