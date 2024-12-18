<script setup>
import HelloWorld from './components/HelloWorld.vue'
import TheWelcome from './components/TheWelcome.vue'
</script>

<template>
  <main>
    <img alt="Lootdoolfs logo" class="logo" src="@/assets/lootis.png"/>
  </main>
</template>

<style scoped>
.logo {
  display: block;
  width: 50%;
  user-select: none;
  -webkit-user-drag: none;
  animation: fade-in ease 1s;
  animation-iteration-count: 1;
}

main{
  display: flex;
  justify-content: center;
}

@media (min-width: 1024px) {
  .logo{
    width: 35%;
  }
}

@keyframes fade-in {
  0% {
    opacity: 0;
    transform: scale(0,0) rotate(-75deg);
  }
  100% {
    opacity: 1;
    transform: scale(1,1) rotate(0deg);
  }
}
</style>
