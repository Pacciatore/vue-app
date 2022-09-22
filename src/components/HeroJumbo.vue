<template>

    <div class="jumbo-container">
        <h2 class="jumbo-title">Questo è un jumbotron!</h2>
        <div class="jumbo-caption">
            Lorem ipsum dolor sit amet consectetur, adipisicing elit. Pariatur eum nostrum nemo, impedit incidunt
            temporibus totam dignissimos! Obcaecati sequi vel veniam non aut mollitia reiciendis impedit debitis
            incidunt tenetur commodi voluptatum unde, earum excepturi, voluptas nisi omnis ipsam error veritatis
            molestias esse? Cupiditate numquam deserunt repudiandae voluptates voluptatibus repellat earum.
        </div>
    </div>

</template>

<script>
export default {
    name: 'HeroJumbo',
}
</script>

<style scoped lang="scss">
.jumbo-container {
    min-height: 80vh;
    background-image: url(../assets/jumbo.png);
    background-position: center;
    background-size: cover;
    background-repeat: no-repeat;

    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
}

.jumbo-caption {
    width: 50%;
}
</style>