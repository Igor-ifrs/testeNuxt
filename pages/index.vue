<template>
    <div class="container">
        <div class="title">
            <div>
                <div>
                    <span>EVERTON</span>
                    <span>MEDEIROS</span>
                </div>
                <TextSlider />
            </div>
        </div>
    </div>
</template>

<script>
export default {};
</script>

<style scoped>
.container {
    height: 100%;
    height: 100vh;
    width: 100vw;
    background-image: url("~assets/img/wewe.jpg");
    background-size: cover;
    background-attachment: fixed;
    border: seashell 5px solid;
    overflow: hidden;
}
.title {
    height: 100%;
    width: 100%;
    display: flex;
    text-align: center;
    justify-content: center;
    align-items: center;
    background-image: linear-gradient(rgba(0, 0, 0, 0.6) 10%, rgba(0, 0, 10, 0.9));
}
span {
    color: seashell;
    font-family: var(--main-font);
    font-size: 5.5rem;
    display: block;
}
</style>
