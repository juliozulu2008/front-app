<script>
import api from '../services/api';
export default {
    name: 'AppContent',
    created() {
        api.get('http://localhost:8000/api/').then((response) => {
            console.log(response.data)
        })
    }

}
</script>
<template>
    <section class="content">
        <div class="main">

        </div>
    </section>
</template>
<style>
.content {
    display: flex;
    align-items: center;
    justify-content: center;
    width: 100%;
    height: 100vh;
}
</style>