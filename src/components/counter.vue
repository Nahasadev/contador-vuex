<template>
    <div class="container">
        <button 
            class="btn btn-success btn-block"
            @click="increment(2)">
            Aumentar contador
        </button>
        <div class="alert alert-secondary text-center mt-3">
            {{counter}}
        </div>
        <button 
            class="btn btn-primary btn-block"
            @click="decrement()">
            Disminuir contador
        </button>
    </div>
</template>

<script>
    import {mapState, mapMutations} from 'vuex'
    export default {
        computed: {
            ...mapState(['counter'])
        },
        methods: {
            ...mapMutations(['increment','decrement'])
        }
    }
</script>

<style lang="stylus">

</style>