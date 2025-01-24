<script setup>
  import Clock from '@/components/Clock.vue';
</script>

<template>
  <main>
    <img alt="Lootdoolfs logo" class="logo" src="@/assets/lootis.png"/>
    <Clock class="clock" />
  </main>
</template>

<style scoped>
.clock{
  width: 95%;
}

.logo {
  display: none;
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
  .clock{
    width: 50%;
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
