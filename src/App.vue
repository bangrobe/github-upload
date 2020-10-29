<template>
<div id="app" class="container">
    <div class="row">
        <div class="col-md-6">
            <ListTask></ListTask>
        </div>
        <div class="col-md-6">
            <CompletedTask></CompletedTask>
        </div>
    </div>
    <GetTask></GetTask>

</div>
</template>

<script>
import GetTask from '@/components/GetTask'
import ListTask from '@/components/ListTask'
import CompletedTask from '@/components/CompletedTask'
export default {
    components: {
        GetTask,
        ListTask,
        CompletedTask
    }
}
</script>

<style>

</style>
