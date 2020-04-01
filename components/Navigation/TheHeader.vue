<template>
  <section class="home-intro">
    <nav>
      <ul>
        <li><nuxt-link to="/about">About</nuxt-link></li>
        <li><nuxt-link to="/">Home</nuxt-link></li>
        <li><nuxt-link to="/posts">Posts</nuxt-link></li>
        <li><nuxt-link to="/admin">Admin</nuxt-link></li>
      </ul>
    </nav>
  </section>
</template>

<script>
export default {};
</script>

<style>
.home-intro {
  height: 20vh;
  padding: 2em;
  background: url("~assets/images/img.png") no-repeat;
  background-position: center;
  background-size: cover;
  margin: 2em 0;
}
ul {
  list-style-type: none;
  display: grid;
  grid-template-columns: repeat(4, max-content);
  grid-column-gap: 20px;
  color: white;
}

a.nuxt-link-active {
  color: black;
}
a {
  color: inherit;
  text-decoration: none;
}
</style>
