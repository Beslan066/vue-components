<template>
    <div class="counter">

        <h3>Counter</h3>
        <div>
            <button 
        v-on:click="counterMinus()"
        >-</button>
            <input type="number" v-bind:value="counter" >
        <button 
        v-on:click="counterPlus()"
        >+</button>
        </div>
    </div>
</template>


<script>
export default {
    name: "CounterComponent",
    data() {
        return {
            counter: 0,
        }
    }, 

    methods: {
        counterMinus() {
            this.counter--
        },

        counterPlus() {
            this.counter++
            console.log(this.counter);
        }
    },
    computed: "",
}
</script>


<style> 

.counter {
    display: flex;
    align-items: center;
    flex-direction: column;
    height: 600px;
    border: 1px solid rgb(9, 116, 41);
    margin-top: 40px;
    border-radius: 10px;
    padding: 10px;
}

h3 {
        color: rgb(9, 116, 41);
    }

</style>