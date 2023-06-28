<script>
import { store } from '../store.js';

export default {
    data() {
        return {
            store
        }
    },    
}
</script>
<template>
    <div class="container mt-4">
        <div class="row">
            <div class="col-6 d-flex">
                <div class="big-circle"></div>
                <div class="small-circle red">
                </div>
                <div class="small-circle yellow"></div>
                <div class="small-circle green"></div>
            </div>
        </div>
    </div>
</template>
<style lang="scss" scoped>

.big-circle{
    height: 100px;
    width: 100px;
    border-radius: 50%;
    background: rgb(0,45,240);
    border: 4px solid white;
    background: linear-gradient(297deg, rgba(0,45,240,1) 28%, rgba(255,255,255,1) 100%);
}

.small-circle{
    height: 50px;
    width: 50px;
    border-radius: 50%;
    border: 4px solid white;
    margin-left: 1em;
}
.red{
    background: rgb(240,0,0);
    background: linear-gradient(297deg, rgba(240,0,0,1) 10%, rgba(255,255,255,1) 95%);
}

.yellow{
    background: rgb(226,240,0);
    background: linear-gradient(297deg, rgba(226,240,0,1) 28%, rgba(255,255,255,1) 90%);
}
.green{
    background: rgb(12,175,11);
    background: linear-gradient(297deg, rgba(12,175,11,1) 28%, rgba(255,255,255,1) 90%);
}
</style>