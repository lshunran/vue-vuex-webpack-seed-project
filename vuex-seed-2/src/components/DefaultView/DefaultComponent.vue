<template>
    <div class="defaultComponent">

    </div>
</template>
<script>
    //  import Vue from 'vue'
    // 在此引入UI库
    import {Field} from 'mint-ui'

    export default {
        name: 'defaultComponent',
        components: {
            // 使用这种方式声明应用的UI组件
            [Field.name]: Field
        },
        data () {
            return {
                // Data
            }
        },
        computed: {
            // 计算属性

        },
        methods: {
            // 方法
        }
    }
</script>
<style>
    .defaultComponent {

    }
</style>
