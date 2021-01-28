<template>
    <div>
        <div class="container bg-home">
            <div class="title-container">
                <div class="title">
                    <h1>EVERTON</h1>
                    <h1>MEDEIROS</h1>
                    <TextSlider />
                </div>
            </div>
        </div>
    </div>
</template>
<script>
export default {};
</script>

<style scoped>
.container {
    height: 100vh;
    width: 100%;
}
.bg-home {
    background-size: cover;
    background-repeat: no-repeat;
    background-image: url("~assets/img/testebg.jpg");
}
.title-container {
    height: 100%;
    width: 100%;
    overflow: hidden;
    background: rgba(0, 0, 0, 0.5);
}
.title h1 {
    font-size: 10rem;
    font-weight: lighter;
    /* color: #f10001; */
    color: seashell;
    text-shadow: #f10001 2px 2px;
}
.title {
    text-align: center;
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -65%);
    padding: 20px;
    /* border-bottom: 5px solid seashell; */
}
@media only screen and (max-width: 600px) {
    .title h1 {
        font-size: 3.2rem;
    }
}
</style>
