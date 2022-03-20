<template>
  <div class="nav nav-shadow">
    <a class="navitem" href="#">Home</a>
    <a class="navitem" href="#">test</a>
    <a class="navitem" href="#">test</a>
    <a class="navitem" href="#">test</a>
    <a class="navitem" href="#">test</a>
  </div>
</template>

<style scoped>
.nav {
  width: 100%;
  z-index: 20;
  display: flex;
  position: -webkit-sticky;
  position: fixed;
  top: 0;
  align-items: center;
  border-bottom: 1px solid #2f2f2f;
  height: 7vh;
  padding: 0.5rem;
  background-color: #1c1c1c;
}

.nav-shadow {
  box-shadow:
    0 1px 1px hsl(0deg 0% 0% / 0.075),
    0 2px 2px hsl(0deg 0% 0% / 0.075),
    0 4px 4px hsl(0deg 0% 0% / 0.075),
    0 8px 8px hsl(0deg 0% 0% / 0.075),
    0 16px 16px hsl(0deg 0% 0% / 0.075);
}

.navitem {
  color: #FFF;
  font-weight: 700;
  margin-right: 1.125rem;
  text-decoration: none;
}

.navitem:hover {
  filter: brightness(80%);
}
</style>
