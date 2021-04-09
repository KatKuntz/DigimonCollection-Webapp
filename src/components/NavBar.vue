<template>
  <v-app-bar app>
    <NavLink exact link="home">Home</NavLink>
    <template class="xsOnly">
      <v-spacer />
      <NavLink link="database">Card Database</NavLink>
      <v-spacer />
      <NavLink link="register" color="primary">Sign Up</NavLink>
      <NavLink link="login" color="success">Log In</NavLink>
    </template>
  </v-app-bar>
</template>

<script>
import NavLink from "./NavLink";

export default {
  components: {
    NavLink,
  },
};
</script>
