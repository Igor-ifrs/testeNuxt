<template>
    <div>
        <div class="container bg-home">
            <div class="title">
                <div>
                    <h1>EVERTON</h1>
                    <h1>MEDEIROS</h1>
                    <TextSlider />
                </div>
            </div>
        </div>
        <div class="container">
            <h1>partete 2</h1>
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
    background-attachment: fixed;
    background-image: url("~assets/img/wewe.jpg");
}
.title {
    height: 100%;
    width: 100%;
    display: flex;
    text-align: center;
    justify-content: center;
    align-items: center;
    background-image: linear-gradient(rgba(0, 0, 0, 0.6) 10%, rgba(0, 0, 10, 0.9));
    /* overflow: hidden; */
}
.title div h1 {
    color: seashell;
    font-size: 5.5rem;
    display: block;
    font-weight: lighter;
}
@media only screen and (max-width: 600px) {
    .title div h1 {
        font-size: 3.5rem;
    }
}
.title div {
    padding: 15px;
}
#__layout > div > div:nth-child(2) > div.container.bg-home > div > div {
    border-bottom: seashell 2px solid;
}
</style>
