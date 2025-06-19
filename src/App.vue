<template>
  <div class="fixed inset-0 overflow-hidden bg-[#030c4d] flex items-center justify-center">
    <!-- Blobs -->
    <div class="absolute w-[400px] h-[400px] bg-[#f8a01b] rounded-full filter blur-3xl opacity-30 animate-blob left-1/3 top-1/4"></div>
    <div class="absolute w-[400px] h-[400px] bg-[#f8a01b] rounded-full filter blur-3xl opacity-20 animate-blob delay-1000 left-1/2 top-2/3"></div>

    <!-- Glass Content -->
    <div class="relative z-10 text-center p-8 rounded-xl backdrop-blur-lg bg-white/10 shadow-xl w-[90%] max-w-md">
      <h1 class="text-4xl md:text-5xl font-bold text-white mb-4">COMING SOON</h1>
      <a
        href="https://svelue.com"
        target="_blank"
        class="text-white text-sm hover:text-yellow-300 transition"
      >
        managed by svelue
      </a>
    </div>
  </div>
</template>

<style scoped>
@keyframes blob {
  0%, 100% {
    transform: translate(0, 0) scale(1);
  }
  50% {
    transform: translate(30px, -30px) scale(1.1);
  }
}

.animate-blob {
  animation: blob 20s infinite;
}

.delay-1000 {
  animation-delay: 1s;
}
</style>
