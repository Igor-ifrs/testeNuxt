<template>
    <dir>
        <Container>
            <h1>teste 1 componente</h1>
        </Container>
        <Container>
            <h1>teste 2 componente</h1>
        </Container>

        <Container>
            <h1>teste 3 componente</h1>
        </Container>
        <Container id="ever">
            <h1>teste 4 componente</h1>
        </Container>
    </dir>
</template>

<script>
export default {};
</script>

<style>
#ever {
    background-image: url("~assets/img/bg_home.jpg");
    background-size: cover;
    font-size: 80px;
    color: greenyellow;
}
</style>
