<template>
    <div class="slide">
        <div class="slide-ex">
            <p class="ctg">LOCUTOR PROFISSIONAL</p>
            <p class="ctg">ANUNCER FIGTH!</p>
            <p class="ctg">RADIALISTA</p>
        </div>
    </div>
</template>

<script>
export default {};
</script>

<style scoped>
.ctg {
    display: flex;
    justify-content: center;
    align-items: center;
}
.slide {
    height: 80px;
    overflow: hidden;
}
.slide-ex {
    animation: slide infinite 8s;
    animation-timing-function: steps(5, end);
}
@keyframes slide {
    0% {
        margin-top: 0px;
    }
    33% {
        margin-top: -80px;
    }
    66% {
        margin-top: -160px;
    }
    100% {
        margin-top: -240px;
    }
}
p {
    color: seashell;
    font-family: var(--main-font);
    font-size: 2rem;
    color: goldenrod;
    height: 80px;
}
</style>
