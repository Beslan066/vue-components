<template>

    

    <div class="computed-block">
        <h2>Computed and watchers</h2>
        {{text}}
    </div>
</template>

<script>
export default {

    name: "ComputedComponent",
    data() {
        return {
            text: "aaa",
        }
    }

}
</script>


<style>

h2 {
    color: rgb(9, 116, 41);
}

.computed-block {
    height: 600px;
    border: 1px solid rgb(9, 116, 41);
    margin-top: 40px;
    border-radius: 10px;
    padding: 10px;
}

</style>