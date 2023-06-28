<script>
export default {
    props:{
        myPokemon: Object
    }
}
</script>
<template>
    <div class="card" :class="myPokemon.type1 === 'Grass'? 'grass' : myPokemon.type1 === 'Water' ? 'water' : myPokemon.type1 === 'Fire'? 'fire': ''">
        <img :src="myPokemon.imageUrl" :alt="myPokemon.name">
        <div>{{ myPokemon.number }}</div>
        <p><strong>{{ myPokemon.name }}</strong></p>
        <div>{{ myPokemon.type1 }}</div>
    </div>
</template>
<style lang="scss">
img{
    width: 120px;
    height: 120px;
    border-radius: 50%;
}

.card{
    display: flex;
    align-items: center;
    margin: 1em 0em;
    padding: 25px 20px;
}

.grass{
    background-color: #DEFDE0 !important
}

.fire{
    background-color: #FDDFDF !important
}

.water{
    background-color: #DEF3FD !important
}
</style>