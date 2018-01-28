<template>
    <div>
        <h1>Server Status: {{status}}</h1>
        <hr>
        <button @click="changeStatus">Change</button>
    </div>
</template>

<script>
export default {
    name: 'app',
    data: function(){
        return {
            status: 'OK'
        }
    },
    methods: {
        changeStatus: function(){
            this.status = "Critical!"
        }
    }
}
</script>
