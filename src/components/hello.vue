<template>
    <div>
        {{msg}}
    </div>
</template>

<script lang="ts">
import {Component, Prop, Vue} from "vue-property-decorator";

@Component
export default class HelloWorld extends Vue {
    //！是为了告诉typescript，msg必须传，{required:true}是告诉vue，msg必须传
    @Prop({required: true}) private msg!: string;
}
</script>

<style scoped>

</style>
