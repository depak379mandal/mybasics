<template>
    <div>
        <div class="text-center">
            First Name
            <input type="text" class="input-group" v-model="firstName">
        </div>
        <div class="text-center">
            Last Name
            <input type="text" class="input-group" v-model="lastName">
        </div>
        <div>
            Full Name <span style="color:red;">{{fullName}}</span>
        </div>
        <button @click="count++">Add 1</button>
        <div>
            Change Something of Count : {{count}}
        </div>
    </div>
</template>

<script>
export default {
    name: 'Form',
    data(){
        return {
            firstName : '',
            lastName : '',
            count : 0,
            }
    },
    computed:{
        fullName(){
            return this.firstName + ' '+ this.lastName;
        }
    }
}
</script>

<style scoped>
    .form-group{
        display: flex;
        justify-content: center;
        align-items: center;
        margin: 1em 0;
        flex-direction: column;
    }
    .text-center{
        text-align: center;
        display: block;
    }
    .input-group{
        border: 1px solid #ddd;
        border-radius: 2px;
        line-height: 2em;
        padding: 0;
        margin: 1em auto;
    }
</style>