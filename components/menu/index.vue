<template>
  <div>
    <div class="btn-menu-container" @click="toggle">
      <div class="btn-menu" :class="{ btnClose: isActive }"></div>
    </div>
    <menu class="menu" :class="{ menuOpen: isActive }" @click="toggle">
      <NuxtLink to="/">INÍCIO</NuxtLink>
      <NuxtLink to="/#exemplos">EXEMPLOS</NuxtLink>
      <NuxtLink to="/teste">GALERIA</NuxtLink>
      <NuxtLink to="/#redes">SIGA-ME!</NuxtLink>
    </menu>
  </div>
</template>

<script>
export default {
  data() {
    return { isActive: false };
  },
  methods: {
    toggle() {
      this.isActive = !this.isActive;
    },
  },
};
</script>

<style scoped>
.btn-menu-container {
  height: 80px;
  width: 80px;
  position: fixed;
  top: 40px;
  right: 60px;
  cursor: pointer;
  transition: all 0.5s linear;
  z-index: 9999;
}
.btn-menu-container:hover {
  transform: scale(1.2);
}
.btn-menu {
  height: 100%;
  width: 100%;
  background: white;
  clip-path: polygon(
    0% 5%,
    100% 5%,
    100% 25%,
    0% 25%,
    0% 40%,
    100% 40%,
    100% 60%,
    0% 60%,
    0% 75%,
    100% 75%,
    100% 95%,
    0% 95%
  );
  transition: clip-path 0.1s linear;
}
.btnClose {
  clip-path: polygon(
    20% 0%,
    0% 20%,
    30% 50%,
    0% 80%,
    20% 100%,
    50% 70%,
    80% 100%,
    100% 80%,
    70% 50%,
    100% 20%,
    80% 0%,
    50% 30%
  );
}
.menu {
  height: 100vh;
  width: 100vw;
  background: black;
  position: fixed;
  top: 0;
  left: 0;
  transform: translate(-100%, 0);
  transition: transform 0.6s ease-in;
  transition-delay: 0.5s;
  display: flex;
  flex-direction: column;
  justify-content: space-around;
  z-index: 1;
}
.menuOpen {
  transform: translate(0, 0);
}
.menu a {
  color: white;
  display: block;
  font-size: 300%;
  text-decoration: none;
  text-align: center;
  padding: 20px;
}
a.nuxt-link-exact-active {
  opacity: 0.5;
}
@media only screen and (max-width: 600px) {
  .menu {
    background: black;
    width: 100%;
  }
  .btn-menu-container {
    height: 40px;
    width: 40px;
    top: 10px;
    right: 10px;
  }
}
</style>
