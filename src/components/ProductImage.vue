<template>
    <div id="showImage">
        <img :src="image" alt="" style="width: 70%;">
        <div style="width: 30px; position: absolute; top: 20px; right: 20px;" :style="`display: ${zoom}`">
            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
                <path stroke-linecap="round" stroke-linejoin="round" d="M21 21l-5.197-5.197m0 0A7.5 7.5 0 105.196 5.196a7.5 7.5 0 0010.607 10.607z" />
            </svg>
        </div>
    </div>
</template>

<script>
    export default {
        name: "ProductImage",
        props: ['image', 'zoom'],
    }
</script>

<style scoped>
    #showImage {
        border: solid 1px;
        border-radius: 10px;
        display: flex;
        justify-content: center;
        align-items: center;
        position: relative;
        overflow: hidden;
    }
</style>