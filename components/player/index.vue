<template>
    <div :id="id" class="player">
        <audio controls :src="src"></audio>
    </div>
</template>

<script>
export default {
    props: {
        src: String,
        id: String,
    },
};
</script>

<style>
.player {
    background: turquoise;
    height: 100px;
}
</style>
