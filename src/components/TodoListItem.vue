<template>
    <li>
        <lavel for="trimmedText">{{ todo.text }}</lavel>
        <input type="checkbox" id="trimmedText" v-model="checkbox">
        <button @click="$emit('remove', todo.id)">삭제</button>
    </li>
</template>

<script>
export default{
    props:{
        todo: {
            type: Object,
            required: true
        }
    }
}
</script>