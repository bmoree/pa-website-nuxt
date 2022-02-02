<template>
  <header class="sitenav">
    <a href="/" class="logo"
      ><img
        src="https://propeller-apps.nl/wp-content/uploads/2019/05/logo-propeller-apps-v4.jpg"
        alt="logo"
      />
    </a>
    <div class="hamburger" @click="open = !open">
      <svg
        xmlns="http://www.w3.org/2000/svg"
        width="24"
        height="24"
        fill="none"
        stroke="currentColor"
        stroke-width="2"
        stroke-linecap="round"
        stroke-linejoin="round"
      >
        <path d="M3 12h18M3 6h18M3 18h18" />
      </svg>
    </div>
    <nav class="main-nav" :class="{ open: open }">
      <a href="/diensten">Diensten</a>
      <a href="/over">Over</a>
      <a href="/blog">Blog</a>
      <a href="/contact">Contact</a>
      <a href="#" class="close" @click="open = !open">
        <svg
          xmlns="http://www.w3.org/2000/svg"
          width="24"
          height="24"
          fill="none"
          stroke="currentColor"
          stroke-width="2"
          stroke-linecap="round"
          stroke-linejoin="round"
        >
          <path d="M18 6 6 18M6 6l12 12" />
        </svg>
      </a>
    </nav>
  </header>
</template>
<script>
export default {
  data() {
    return {
      open: false,
    };
  },
};
</script>
