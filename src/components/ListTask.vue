<template>
<div id="list-tasks">
    <div class="panel panel-default">
        <div class="panel-heading my-task">
            <h3 class="panel-title">My Tasks <span class="task-length" v-if="tasks.length > 0">{{tasks.length}}</span></h3>
        </div>
        <div class="panel-body">
            <ul class="list-group">
                <li class="list-group-item" v-for="(task, index) in tasks" v-bind:key="index">
                    <img src="https://lazi.vn/files/large/5a64450874df215" alt="" width="54">
                    {{task.body}}
                    <div class="btn-group">
                        <button type="button" class="btn btn-default btn-sm" href="#edit" role="button">Edit</button>
                        <button type="button" class="btn btn-success btn-sm" href="#complete" role="button">Complete</button>
                        <button type="button" class="btn btn-danger btn-sm" href="#remove" role="button">Remove</button>
                    </div>
                </li>
            </ul>
        </div>
    </div>

</div>
</template>

<script>
export default {}
</script>

<style>

</style>
