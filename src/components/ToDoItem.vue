<template>
    <div class="flex gap-2 items-center px-4 py-2">
        <label class="flex gap-2 items-center select-none cursor-pointer">
            <input type="checkbox">
            <p class="opacity-80">{{ text }}</p>
        </label>
        <div class="flex gap-2 ml-auto">
            <small class="text-orange-400 cursor-pointer hover:underline uppercase">Edit</small>
            <small class="text-red-600 cursor-pointer hover:underline uppercase">Delete</small>
        </div>
    </div>
</template>

<script setup>
    //eslint-disable-next-line
    defineProps(["text"])
</script>

<style scoped>

</style>