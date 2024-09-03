<template>
    <view>
        home
        <br>
        <icon type="success"></icon>
        <br>
        <text>不可选文字\n</text>
        <text :selectable="true">可选文字</text>
        <br>
        <image src="../../static/img/4.jpg" mode="aspectFill"></image>
    </view>
</template>

<script>
    export default {
        data() {
            return {
                
            }
        },
        methods: {
            
        }
    }
</script>

<style lang="scss">
    image{
        background-color: yellow;
    }

</style>
