<template>
    <div class="search-blok">
        <h3>Поиск Vue</h3>
        
        <div class="search-input-block">
            <label for="search-input">Найдите пользователя из учетной книги</label>
            <input type="search" name="search-input">
        </div>

        <div class="users">
            <ul>
                <li></li>
                <li></li>
                <li></li>
            </ul>
        </div>
    </div>
</template>


<script>
export default {
    name: "SearchList",
    data() {
        return {
            users: ["Beslan","Adam","Timur", "Musa"],
        }

    }
}
</script>


<style>
    .search-blok {
        height: 400px;
        border: 1px solid rgb(9, 116, 41);
        margin-top: 40px;
        border-radius: 10px;
        padding: 10px;
    }

    h2 {
        color: rgb(9, 116, 41);
    }

    .search-input-block {
        display: flex;
        flex-direction: column;
    }

    label {
        color: rgba(128, 128, 128, 0.808);
    }

   

</style>