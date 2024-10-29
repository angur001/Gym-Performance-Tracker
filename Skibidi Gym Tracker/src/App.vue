<template>
   <div class="container">
    <HeaderSection />
    <GroupListing :exerciseList="Data"/>
  </div>
</template>

<script setup>
import HeaderSection from './components/HeaderSection.vue'
import GroupListing from './components/GroupListing.vue'

let Data = {
    "Monday": [
        'Bench Press',
        'Incline Dumbbell Press',
        'Chest Flyes',
        'Push-Ups',
        'Tricep Dips'
    ],
    "Tuesday": [
        'Squats',
        'Leg Press',
        'Lunges',
        'Leg Extensions',
        'Calf Raises'
    ],
    "Wednesday": [
        'Pull-Ups',
        'Lat Pulldowns',
        'Bent-Over Rows',
        'Seated Cable Rows',
        'Deadlifts'
    ],
    "Thursday": [
        'Overhead Shoulder Press',
        'Lateral Raises',
        'Front Raises',
        'Reverse Pec Deck',
        'Shrugs'
    ],
    "Friday": [
        'Bicep Curls',
        'Hammer Curls',
        'Preacher Curls',
        'Tricep Extensions',
        'Skull Crushers'
    ],
    "Saturday": [
        'Deadlifts',
        'Romanian Deadlifts',
        'Back Extensions',
        'Pull-Throughs',
        'Leg Curls'
    ],
    "Sunday": [
        'Yoga',
        'Foam Rolling',
        'Stretching Routine',
        'Core Workouts (e.g., Plank)',
        'Light Cardio (e.g., Walking, Cycling)'
    ]
};
</script>
