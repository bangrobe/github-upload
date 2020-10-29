<template>
<div id="completed-tasks">
    <div class="card">
        <div class="card-body">
            <h5 class="card-title">
                Completed<span class="completed-length" v-if="completed.length > 0">{{complete.length}}</span>
            </h5>
            <ul class="list-group">
                <li class="list-group-item complete-list" v-for="(task,index) in completed" v-bind:key="index">{{task.body}}</li>
                <button type="button" class="btn btn-danger btn-sm remove-completed">Remove</button>
            </ul>
        </div>
    </div>
</div>
</template>

<script>
export default {

}
</script>

<style>

</style>
