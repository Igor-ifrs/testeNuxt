<template>
  <div class="slide">
    <div class="slide-ex">
      <p>LOCUTOR PROFISSIONAL</p>
      <p>ANUNCER FIGTH!</p>
      <p>RADIALISTA</p>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.slide {
  height: 80px;
  overflow: hidden;
  -webkit-box-shadow: 3px 3px 3px 0px rgba(241, 0, 0, 1);
  -moz-box-shadow: 3px 3px 3px 0px rgba(241, 0, 0, 1);
  box-shadow: 3px 3px 3px 0px rgba(241, 0, 0, 1);
}
.slide-ex {
  animation: slide infinite 9s steps(3);
}
@keyframes slide {
  to {
    margin-top: -240px;
  }
}
.slide-ex:hover {
  animation-play-state: paused;
}
.slide-ex p {
  color: seashell;
  font-size: 2.2rem;
  /* color: goldenrod; */
  color: #f10001;
  height: 80px;
  display: flex;
  justify-content: center;
  align-items: center;
  background: seashell;
}
@media only screen and (max-width: 600px) {
  .slide-ex p {
    font-size: 1.5rem;
  }
}
</style>
