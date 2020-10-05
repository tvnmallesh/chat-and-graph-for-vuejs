<template>
  <div>
    <mdb-navbar position="top" dark color="primary" scrolling>
      <mdb-navbar-brand href="#"><img alt="MDB logo" src="../assets/logo.png"></mdb-navbar-brand>
      <mdb-navbar-toggler>
        <mdb-navbar-nav>
          <mdb-nav-item href="#" waves-fixed>Home</mdb-nav-item>
          <mdb-nav-item href="#" waves-fixed>Features</mdb-nav-item>
          <mdb-nav-item href="#" waves-fixed>Pricing</mdb-nav-item>
          <mdb-dropdown tag="li" class="nav-item">
            <mdb-dropdown-toggle
              tag="a"
              navLink
              color="primary"
              slot="toggle"
              waves-fixed
              >Dropdown</mdb-dropdown-toggle
            >
            <mdb-dropdown-menu>
              <mdb-dropdown-item>Action</mdb-dropdown-item>
              <mdb-dropdown-item>Another action</mdb-dropdown-item>
              <mdb-dropdown-item>Something else here</mdb-dropdown-item>
            </mdb-dropdown-menu>
          </mdb-dropdown>
        </mdb-navbar-nav>
        <form>
          <mdb-input
            type="text"
            class="text-white"
            placeholder="Search"
            aria-label="Search"
            label
            navInput
            waves
            waves-fixed
          />
        </form>
      </mdb-navbar-toggler>
    </mdb-navbar>
    <div style="height: 110vh">
      <div class="view intro-2">
        <div class="full-bg-img">
          <div class="mask rgba-white-strong">
            <div class="container flex-center">
              <div class="dark-grey-text">
                <h2 class="font-weight-bold">
                  Fixed navbar
                </h2>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
  import {
    mdbNavbar,
    mdbNavItem,
    mdbNavbarNav,
    mdbNavbarToggler,
    mdbDropdown,
    mdbDropdownItem,
    mdbDropdownMenu,
    mdbDropdownToggle,
    mdbInput,
    mdbNavbarBrand
  } from "mdbvue";
  export default {
    name: "NavigationPage",
    components: {
      mdbNavbar,
      mdbNavItem,
      mdbNavbarNav,
      mdbNavbarToggler,
      mdbDropdown,
      mdbDropdownItem,
      mdbDropdownMenu,
      mdbDropdownToggle,
      mdbInput,
      mdbNavbarBrand
    },
  };
  </script>