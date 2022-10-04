<template>
    <div class="box">
    <div class="title">{{ title }}</div>
    <div class="message">
        {{msg}}
    </div>
    <hr size="2" width="50%" align="left">
    </div>
</template>
<script lang="ts">
import { Options, Vue } from 'vue-class-component';

@Options({
    props: {
    title: String,
    msg: String
    }
})
export default class CompBox extends Vue {
    title!: string
    msg!: string
}
</script>
<style scoped>
    .box {
        margin-left: 15%;
        text-align: left;
        width: 1000px;
        left: 20%;
        color: rgb(255, 255, 255);
    }
    .title {
        font-size: 48px;
    }

    .message{
        font-size: 36px;
    }
</style>