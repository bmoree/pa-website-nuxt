<template>
  <main>
    <section class="hero">
      <div class="container">
        <div>
          <h1 class="text-4xl">Blog</h1>
        </div>
      </div>
    </section>
    <div class="container md:flex -mx-2">
      <template v-if="articles.length">
        <div
          class="p-6 mx-2 my-2 md:w-1/2 ;g:w-1/3"
          v-for="(article, index) in articles"
          :key="index"
        >
          <img :src="`https://picsum.photos/id/${index}/600/400`" alt="" />
          <a :href="article.path" class="block mt-4 text-sky-700 font-bold">{{
            article.title
          }}</a>
          <nuxt-content :document="{ body: article.excerpt }" />
        </div>
      </template>
    </div>
  </main>
</template>
<script>
export default {
  async asyncData({ $content, params }) {
    const articles = await $content('blog').fetch();

    return {
      articles,
    };
  },
};
</script>
