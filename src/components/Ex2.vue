<script setup>
    import { ref } from 'vue'

    // Add code here
    /* method 1 */
    import me from '/assets/me.png'

    const obj = {
        src: '/assets/me.png',
        width: "200",
        height: "200"
    }

    /* method 2 */
    const width=ref("200")
    const height=ref("200")    
    const myImg = ref('/assets/me.png')

    /* method 3 */

    const img = {
        src: '/assets/me.png',
        width:"200",
        height:"200"
    }

</script>

<template>

    <!-- Add code here -->
    <img v-bind:src="myImg" :width="width" :height="height"/>

    <img v-bind="obj" />


</template>
