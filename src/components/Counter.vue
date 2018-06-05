<template>
    <div>
        <button class="btn btn-primary" @click="asyncIncrement({by: 50, durations: 500})">Increment</button>
        <button class="btn btn-primary" @click="asyncDecrement({by: 50, duration: 500})">Decrement</button>
    </div>
</template>

<script>
    import { mapMutations } from 'vuex';
    export default {
        methods: {
            ...mapMutations([
                'asyncIncrement',
                'asyncDecrement'
            ])
        }
    }
</script>