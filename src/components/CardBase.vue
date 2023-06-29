<script lang="ts">
import { defineComponent } from 'vue';
import Portrait from './Portrait.vue';
export default defineComponent({
    components: { Portrait },
    methods: {
        moveImage(){
            var portrait = document.getElementById("portrait");
            portrait?.classList.toggle("moved");
        }
    }
})


</script>

<template>
    <div class="w-[600px] h-[800px] flex flex-col justify-center items-center">
        <div id="cardbase" class="flex justify-start items-start p-4 min-w-[300px] w-[600px] h-[400px] shadow drop-shadow-lg rounded-xl bg-white">
            <span id="portrait" v-on:click="moveImage" class="static"><Portrait /></span>
        </div>
    </div>
</template>

<style>
    .static {
        transform: translateY(0);
        transition: transform 0.3s ease-in;
    }
    
    .static.moved {
        transform: translateY(-250px);
    }

</style>