<template>
    <div>
        <h1>Hello world!</h1>

        {{ name }}

        <input type="text" v-model="name" @input="handleUpdate">
    </div>

</template>

<script setup>

import { ref } from 'vue';

const emit = defineEmits(['updateName'])

const handleUpdate = (event) => {
    emit('updateName', event.target.value)
}
const name = ref('')


</script>
