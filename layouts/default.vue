<template>
    <div>
        <Nuxt />
        <menu class="lk">
            <NuxtLink to="#ever">everton</NuxtLink>
            <NuxtLink to="/">Home page</NuxtLink>
        </menu>
    </div>
</template>

<style>
.lk {
    position: fixed;
    top: 0;
    display: block;
    background: orangered;
    height: 100px;
}
</style>
