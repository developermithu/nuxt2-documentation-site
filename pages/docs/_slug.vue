<template>
  <div>
    <Header />

    <main class="flex">
      <!-- Sidebar -->
      <div class="py-5 px-8 border-r-2 border-gray-300 w-2/12">
        <Sidebar />
      </div>

      <!-- Content -->
      <div class="py-5 px-8 w-10/12">
        <pre>{{ docs.title }}</pre>
        <article class="prose">
          <nuxt-content :document="docs" />
        </article>
      </div>
    </main>
  </div>
</template>

<script>
export default {
  async asyncData({ $content, params }) {
    const docs = await $content("documentation", params.slug).fetch();
    return { docs };
  },

  head() {
    return {
      title: this.docs.title,
      meta: [
        { hid: "description", name: "description", content: this.docs.description },
        // Open Graph
        { hid: "og:title", name: "og:title", content: this.docs.title },
        { hid: "og:description", name: "og:description", content: this.docs.description },
        // Twitter Card
        { hid: "twitter:card", name: "twitter:card", content: 'summery' },
        { hid: "twitter:site", name: "twitter:site", content: '@developermithu' },
        { hid: "twitter:title", name: "twitter:title", content: this.docs.title },
        { hid: "twitter:description", name: "twitter:description", content: this.docs.description },
        { hid: "twitter:image", name: "twitter:image", content: this.docs.image },
        { hid: "twitter:player", name: "twitter:player", content: this.docs.video },
      ],
    };
  },
};
</script>