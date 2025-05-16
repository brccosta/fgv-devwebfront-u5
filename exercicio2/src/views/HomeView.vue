<template>
  <main>
    <TheWelcome />
    <div class="users">
      <h2>Usuários da Plataforma</h2>
      <div class="user-links">
        <router-link :to="'/user/1'">João Silva</router-link> |
        <router-link :to="'/user/2'">Maria Souza</router-link> |
        <router-link :to="'/user/3'">Carlos Oliveira</router-link>
      </div>
    </div>
  </main>
</template>

<style scoped>
.users {
  margin-top: 20px;
  text-align: center;
}
.user-links {
  margin-top: 10px;
}
</style>