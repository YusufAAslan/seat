<template>
    <MainMenu />
    <div class="container text-center mt-5">
        <h1>Models</h1>
        <img src="..\assets\car.png" class="img-fluid" alt="Car Model">
        <h2>IBIZA</h2>
        <p>193.500 TL'den başlayan fiyatlarla</p>
        <button class="btn btn-primary">Select</button>
    </div>
</template>

<script>
export default {
    name: "Models",
};
</script>

<style scoped>
.container {
    max-width: 600px;
    margin: auto;
}

h1 {
    font-size: 36px;
    margin-bottom: 20px;
}

h2 {
    font-size: 30px;
    margin-top: 20px;
}

p {
    font-size: 18px;
    margin: 10px 0 20px;
}

button {
    margin-top: 20px;
}
</style>
