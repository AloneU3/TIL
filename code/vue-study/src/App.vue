<template>
    <form v-on:submit.prevent>
        <div v-bind="number">
            {{ number }}
        </div>
        <button v-on:click="pl"> + </button>
    </form>
</template>

<script>
export default {
    data: function() {
        return {
            number: 0
        }
    },
    watch: {
        number: function() {
        }
    },
    methods: {
        pl: function() {
            this.number = this.number + 1;
        }
    }
}
</script>

<style>

</style>
