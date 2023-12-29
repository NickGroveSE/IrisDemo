<script setup>

    defineProps({
        name: String,
        artist: String,
        imgurl: String,
        colors: Object
    })

</script>

<template>

    <div>
        <img class="song-element album-art" :src="imgurl">
        <div class="song-element song-details">
            <div class="name">{{ name }}</div>
            <div class="artist">{{ artist }}</div>
        </div>
        <a class="song-element colors-container" href="https://coolors.co/">
            <div 
                class="color"
                v-for="color in colors"
                :style="`background-color: #${color}`"
            ></div>
        </a>
    </div>

</template>

<style scoped>

    .song-element {
        height: 30px;
        display: inline-block;
        vertical-align: top;
    }

    .album-art {
        width: 30px;
    }

    .song-details {
        width: 190px;
        margin-left: 10px;
    }

    .name {
        font-size: 12px;
        font-weight: 700;
        color: var(--text);
    }

    .artist {
        font-size: 12px;
        color: var(--text-accent);
    }


    .colors-container {
        width: 150px;
        float: right;
    }

    .color {
        width: 10px;
        height: 30px;
        float: right;
        vertical-align: top;
    }

    .colors-container:hover .color {
        width: 30px;
        transition: 0.5s;
    }

</style>