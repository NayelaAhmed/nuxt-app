<template>
  <b-navbar
    toggleable="md"
    type="dark"
    variant="info">
    <b-navbar-brand><NuxtLink to="/">Home</NuxtLink></b-navbar-brand>
    <b-navbar-nav>
      <b-nav-item><NuxtLink to="/HandMadeCards">Hand-made Cards</NuxtLink></b-nav-item>
      <b-nav-item><NuxtLink to="/Pricing">Pricing</NuxtLink></b-nav-item>
      <b-nav-item><NuxtLink to="/CardGrid">Grid</NuxtLink></b-nav-item>
       <b-nav-item><NuxtLink to="/Movies">Movies</NuxtLink></b-nav-item>
    </b-navbar-nav>
  </b-navbar>

  
</template>
<script>
export default {
  name: 'Navbar'
};
</script>