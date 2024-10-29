<template>
    <div class="input-group">
        <ul id="group-list">
            <li v-for="groupName in Object.keys(exerciseList)">
                <p> {{groupName}} <Group :listOfExercises="exerciseList[groupName]"/> </p>
            </li>
        </ul>
    </div>
</template>

<script setup>  
import Group from './Group.vue'

const props = defineProps({
    exerciseList: {
        type: Object,
        required: true,
    },
});
</script>