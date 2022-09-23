<template>
    <div>
        <div class="flex gap-2">
            <input v-model="text" type="text" placeholder="Add List Item" class="w-full block border px-2 outline-none">
            <button 
                @click="addMyItem()" 
                class="bg-blue-500 text-white px-8 py-2 cursor-pointer hover:bg-slate-600">ADD</button>
        </div>
    </div>
</template>

<script setup>
    import { ref } from "vue"
    const text = ref('')

    //eslint-disable-next-line
    const props = defineProps(["xx"])

    function addMyItem()
    {
        if(text.value.trim() !== ''){
            props.xx(text.value)
        }

        text.value = ''
    }
</script>

<style scoped>
    
</style>