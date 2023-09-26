<template>
    <div>
        <header>
            <h1>
                {{ propsdata }}
            </h1>
            <button v-on:click="sendEvent">클릭</button>
        </header>
    </div>
</template>

<script>
    export default {
        data(){
            return{
                header : '에베베벱!!'
            }
        },
        methods:{
            sendEvent(){
                this.$emit('renew');
            }
        },
        props:['propsdata']
    }
</script>

<style lang="scss" scoped>

</style>