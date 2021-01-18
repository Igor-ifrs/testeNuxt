<template>
    <h1>pagina teste</h1>
</template>

<script>
export default {
    transition: "home",
};
</script>

<style>
h1 {
    text-align: center;
    color: tomato;
    font-size: 200px;
}
.home-enter-active,
.home-leave-active {
    transition: opacity 0.5s;
}
.home-enter,
.home-leave-active {
    opacity: 0;
}
</style>
