<template>
    <ul>
        <li v-for="exercise in listOfExercises" :key="exercise">
            <p class='btn'> {{exercise}} </p>
        </li>
    </ul>

    <!-- <input type="text" id="new-exercise" placeholder="Add new exercise..." />
    <button id="add-exercise-btn">+</button> -->

</template>

<script setup>
import { defineProps } from 'vue';

const props = defineProps({
    listOfExercises: {
        type: Array,
        required: true,
    },
});
</script>