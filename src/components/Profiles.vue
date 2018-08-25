<template>
    <main>
        <section id="profiles-container">
            <h2>Profiles</h2>
            <ul id="profiles">
                <Card v-for="dino in dinosArray" :key='dino.id' :dino='dino' />
            </ul>
        </section>
    </main>
</template>

<script>
import Card from './Card'

export default {
    name: 'Profiles',
    components: {
        Card
    },
    props:['dinosArray']
}
</script>

<style>
main {
    grid-row: 2/3;
}

main section {
    padding: 0 20px 0 20px;
    display: grid;
    grid-template-columns: repeat(auto-fit, x100);
    grid-gap: 10px;
    margin: 0 auto;
    width: 50%;
}

small {
    color: black;
    font-size: .5rem;
    margin-left: 10px;
}

p {
    font-size: .8rem;
}
</style>
