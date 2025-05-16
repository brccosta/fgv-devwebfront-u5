<script setup lang="ts">
import { useRoute } from 'vue-router';
const route = useRoute();
</script>

<template>
    <div class="user-profile">
        <h1>Perfil do Usuário</h1>
        <div class="profile-card">
            <p><strong>ID do Usuário:</strong> {{ route.params.id }}</p>
            <p><strong>Nome:</strong> Usuário {{ route.params.id }}</p>
            <p><strong>Email:</strong> usuario{{ route.params.id }}@exemplo.com</p>
        </div>
        <router-link to="/" class="back-link">Voltar para Home</router-link>
    </div>
</template>

<style scoped>
.user-profile {
    max-width: 600px;
    margin: 20px auto;
    padding: 20px;
}

.profile-card {
    background-color: #f5f5f5;
    padding: 15px;
    border-radius: 8px;
    margin: 15px 0;
}

.back-link {
    display: inline-block;
    margin-top: 10px;
}
</style>