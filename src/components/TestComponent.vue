<template>
    <div class="test-block">
        <form >
        <label for="email">Введите email</label>
        <input type="text" class="email" name="email" id="email" 
            v-bind:value="email"
            @input="emailInputVal($event.target.value)"
        >
            <br/>
        <label for="password">Введите пароль</label>
        <input type="password" name="password" id="password">
    </form>

    <span>{{email}}</span>
        
        
    </div>
</template>

<script>
    export default {
        name: "TestComponent",
        data() {
            return {
                email: "test@mail.com", 
            }
        },

        methods: {
            emailInputVal(value) {
                this.email = value
            }
        }
    }
</script>

<style>

    .test-block {
        display: flex;
        flex-direction: column;
        height: 600px;
        border: 1px solid rgb(9, 116, 41);
        margin-top: 40px;
        border-radius: 10px;
        padding: 10px;
    }

    form {
        display: flex;
        flex-direction: column;
        
    }

    input {
        width: 200px;
    }

    .counter {
        margin-top: 40px;
    }

    span {
        font-weight: 700;
        margin-top: 40px;
    }

    
</style>