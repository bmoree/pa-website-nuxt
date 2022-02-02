<template>
  <main>
    <section class="hero">
      <div class="container">
        <div>
          <h1>{{ article.title }}</h1>
        </div>
      </div>
    </section>
    <nuxt-content :document="article" class="blog-content container" />
  </main>
</template>
<script>
export default {
  async asyncData({ $content, params }) {
    const article = await $content('blog', params.slug).fetch();

    return {
      article,
    };
  },
};
</script>
<style scoped>
.container {
  max-width: 640px;
  margin: 0 auto;
}
</style>
