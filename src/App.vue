<template>
  <div id="app">
    <header id="header">
      <div class="logo">Logo / Title</div>
      <nav id="nav">
        <router-link :to="{ name: 'Home' }">Home</router-link>
        <router-link :to="{ name: 'Database' }">Database</router-link>
        <router-link :to="{ name: 'Login' }">Log In</router-link>
      </nav>
    </header>
    <router-view />
  </div>
</template>

<style>
#header {
  display: flex;
  background-color: lightblue;
  height: 2rem;
}

#header .logo {
  flex-grow: 1;
  align-self: center;
  margin-left: 1rem;
}

#nav {
  display: flex;
  justify-content: space-between;
  align-items: flex-start;
  flex-grow: 0.2;
  margin-right: 1rem;
}

#nav a {
  text-decoration: none;
  padding: 5px 15px;
}

#nav a.router-link-exact-active {
  background-color: lightskyblue;
  align-self: stretch;
}
</style>
