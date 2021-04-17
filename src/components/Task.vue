<template>
    <h3> {{ task.text }} </h3>
    
</template>

<script>
export default {
    name:'Task',
    props:{
        task: Object,
    },
}
</script>
<style scoped>
.task {
    background: #f4f4f4;
    margin: 5px;
    padding: 10px 20px;
    cursor: pointer;
}
.task.reminder {
    border-left: 5px solid green;
}

.task h3 {
    display: flex;
    align-items: center;
}
</style>