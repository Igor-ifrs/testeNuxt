<template>
    <div>
        <!-- <Player id="qualquerId" src="https://www.w3schools.com/html/horse.mp3"></Player> -->
        <div class="container">
            <div class="title">
                <div>
                    <h1>EVERTON</h1>
                    <h1>MEDEIROS</h1>
                    <p>LOCUTOR PROFISSIONAL</p>
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
    height: 100%;
    height: 100vh;
    width: 100vw;
    background-image: url("~assets/img/wewe.jpg");
    background-size: cover;
    background-attachment: fixed;
    border: greenyellow 5px solid;
}
.title {
    background-image: radial-gradient(rgba(0, 0, 0, 0.8) 40%, rgba(0, 0, 0, 0.5));
    height: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
    color: white;
    text-align: center;
    border: pink 5px solid;
}
.title h1 {
    font-weight: lighter;
    font-size: 5rem;
}
.title p {
    padding: 20px;
    font-size: 22pt;
    border-bottom: 4px solid seashell;
}
p {
    color: goldenrod;
}
</style>
