<template>
    <div class="backdrop">
        <div class="modal" :class="{sale: theme === 'sale'}">
            <h1>{{header}}</h1>
            <p>{{opis}}</p>
        </div>
    </div>
</template>
<script>
export default {
    props: ['header', 'opis', 'theme']
}
</script>
<style scoped>
    h1 {
        color: red;
    }
    .modal {
        width: 400px;
        padding: 20px;
        margin: 100px auto;
        background: white;
        border-radius: 10px;
    }
    .backdrop {
        top: 0;
        position: fixed;
        background: rgba(0,0,0,0.5);
        width: 100%;
        height: 100%;
    }


</style>