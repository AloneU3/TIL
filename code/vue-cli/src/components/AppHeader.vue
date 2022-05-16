<template>
    <header>
        <h1>{{ propsdata }}</h1>
        <button v-on:click="sendEvent">send</button>
    </header>
</template>

<script>
export default {
    props: ['propsdata'],
    methods: {
        sendEvent: function() {
            this.$emit('renew'); //버튼을 클릭 시 상위 컴포넌트에 header이름을 바꿈
        }
    }
}
</script>

<style>

</style>