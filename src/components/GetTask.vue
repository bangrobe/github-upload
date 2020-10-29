<template>
<div id="get-tasks">
    <form v-on:submit.prevent="addTask">
        <input class="form-control" v-bind:value="newTask" v-on:change="getTask" placeholder="I need to..." />
        <br />
        <button type="submit" class="btn btn-primary"><i class="fa fa-plus"></i>New</button>
    </form>
</div>
</template>

<script>
import Vuex from 'vuex'
export default {
    methods: {
        getTask(e) {
            this.$store.dispatch('getTask', e.target.value) //getTask la event, e.target.value la payload cua event
        },
        addTask(e) {
            e.preventDefault();
            this.$store.dispatch('addTask')
            this.$store.dispatch('clearTask')
        }
    },
    computed: {
        newTask() {
            return this.$store.getters.newTask
        }
    }
}
</script>

<style>

</style>
