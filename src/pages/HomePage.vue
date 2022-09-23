<template>
    <div class="grid gap-6 mx-auto w-1/3 my-10">

        <AddToDo :xx="addItem" />

        <ToDoFilter/>
        
        <div class="border">
            <ToDoItem 
                v-for="(todo, index) in todoList"
                :key="index"
                :text="todo"
                class="border-b hover:bg-red-100" />
        </div>
    </div>
</template>


<script setup>
    import { ref } from 'vue'
    import ToDoFilter from '@/components/ToDoFilter.vue';
    import ToDoItem from '@/components/ToDoItem.vue';
    import AddToDo from '@/components/AddToDo.vue';

    const todoList = ref([])

    function addItem(text)
    {
        todoList.value.push(text)
    }
</script>


<style scoped>

</style>