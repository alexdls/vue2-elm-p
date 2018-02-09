<template>
    <div>
        home页面
        <loading v-show="showLoading"></loading>
    </div>
</template>

<script>
    import loading from '@/components/common/loading'

    export default {
        name: "home",
        data(){
            return{
                showLoading: true //加载动画
            }
        },
        components: {
            loading
        },
        mounted() {
            setTimeout(() => {
                this.showLoading = false;
            }, 5000)
        }

    }
</script>

<style scoped>

</style>