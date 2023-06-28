<script>
import AppCards from './AppCards.vue'

import { store } from '../store.js';

export default {
    components:{
        AppCards
    },
    data() {
        return {
            store
        }
    }
}
</script>
<template>
 <div class="container my-4">
        <div class="row row-content">
            <div v-for="(pokemon, index) in store.listOfPokemon" :key="index" class="col-6 col-md-4 col-lg-3">
                <AppCards :myPokemon="pokemon" />
            </div>
        </div>
    </div>
</template>
<style lang="scss" scoped>
.container{
    display: flex;
    justify-content: center;
    align-items: center;
    padding: 2.7em 1.5em;
    background-color: white;
    border-radius: 18px;
    .row-content{
        background-color: #4C5157;
        justify-content: center;
        padding: 0.8em 0em;
        height: 500px;
        overflow: auto;
        width: 100%;
    }
}

</style>