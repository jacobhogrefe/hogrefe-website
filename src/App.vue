<script setup>
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <div>
    <nav>
      <router-link to="/">Home</router-link>
      <router-link to="/projects">Projects</router-link>
      <router-link to="/about">About</router-link>
    </nav>
    <router-view />
  </div>
</template>

<style scoped>

nav {
  font-family: 'San Francisco Bold';
  font-size: 30px;
  display: flex;
  justify-content: center;
  align-items: center;
}

.nav-links {
  list-style: none;
  margin: 10;
  padding: 5px;
  display: flex;
  justify-content: flex-end;
}

.nav-links li {
  margin: 0 10px;
  text-decoration: none;
  color: rgb(82, 81, 81);
}

.nav-links li a {
  text-decoration: none;
  color: #090909;
  padding: 10px 20px;
  font-size: 18px;
  border-radius: 0.5em;
  background: #e8e8e8;
  border: 1px solid #e8e8e8;
  transition: all .3s;
  box-shadow: 6px 6px 12px #c5c5c5,
              -6px -6px 12px #ffffff;
}

.nav-links li a:hover {
  border: 1px solid white;
  color: #aaaaaa;
}

.nav-links li a:active {
  color: #4f4f4f;
  box-shadow: 4px 4px 12px #c5c5c5,
              -4px -4px 12px #ffffff;
}

.nav-links li a img{
  transition: all .3s;
  position: relative;
  top: 8px;
}

.nav-links li a:hover img{
  filter: invert(71%) sepia(15%) saturate(11%) hue-rotate(315deg) brightness(94%) contrast(85%);
}

.nav-links li a:active img {
  filter: invert(27%) sepia(0%) saturate(2161%) hue-rotate(201deg) brightness(98%) contrast(82%);
}
</style>
