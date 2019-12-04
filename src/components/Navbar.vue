<template>
  <nav class="uk-navbar-container uk-margin navbar_top">
    <div class="uk-container">
      <div class="uk-navbar-left ">
        <g-link class="uk-navbar-item  uk-logo" href="/">
          <g-image src="~/assets/images/impose-logo.png" width="150" />
        </g-link>
        <g-link class="uk-navbar-item nav_link" exact to="/">Home</g-link>
        <g-link class="uk-navbar-item nav_link" to="/About/">About Me</g-link>
        <g-link class="uk-navbar-item nav_link" to="/Posts/">Posts</g-link>
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  name: "Navbar"
};
</script>

<style scoped>
.navbar_top{
  height: 50px;

}
.nav_link {
  text-transform: uppercase;
  font-weight: 500;
  font-size: 13px;
  position: relative; 
  min-width: 50px;
  height: 50px;
}
.nav_link:hover {
  text-decoration: none;
  color: gainsboro;
}
.nav_link.active::before {
  content: "";
  width: 100%;
  height: 2px;
  position: absolute;
  bottom: 0px;
  background-color: black;
}
</style>
