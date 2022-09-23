<template>
    <div class="grid gap-6 mx-auto w-1/3 my-10">
        <AddToDo/>
        <ToDoFilter/>
        <div class="border">
            <ToDoItem class="border-b hover:bg-red-100" />
            <ToDoItem class="border-b hover:bg-red-100" />
            <ToDoItem class="border-b hover:bg-red-100" />
            <ToDoItem class="border-b hover:bg-red-100" />
            <ToDoItem class="border-b hover:bg-red-100" />
            <ToDoItem class="border-b hover:bg-red-100" />
            <ToDoItem class="hover:bg-red-100" />
        </div>
    </div>
</template>


<script setup>
    import ToDoFilter from '@/components/ToDoFilter.vue';
    import ToDoItem from '@/components/ToDoItem.vue';
    import AddToDo from '@/components/AddToDo.vue';

</script>


<style scoped>

</style>