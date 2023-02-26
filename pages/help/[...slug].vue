<script setup lang="ts">
const { path } = useRoute();
const { prev, next } = useContent();
const { data: pages } = await useAsyncData(`help`, () =>
  queryContent({ where: { _path: { $contains: '/help/' } } }).find()
);
console.log(pages);
const groups = computed(() => {
  const groups = [...new Set(pages.value.map((p) => p._dir))];
  return groups.map((title) => ({
    title: title.replaceAll('-', ' '),
    pages: pages.value.filter((p) => p._dir === title),
  }));
});
</script>

<template>
  <div class="help">
    <div class="sidebar">
      <div class="group" v-for="group in groups" :key="group.title">
        <div class="group-title">{{ group.title }}</div>
        <template v-for="page in group.pages">
          <router-link class="item" :to="page._path">
            {{ page.title }}
          </router-link>
          <template v-if="path.includes(page._path)">
            <router-link
              class="toc"
              v-for="link in page.body.toc.links"
              :to="`${page._path}/#${link.id}`"
              :key="link.text"
            >
              {{ link.text }}
            </router-link>
          </template>
        </template>
      </div>
    </div>
    <main>
      <ContentDoc />
      <div class="paging">
        <NuxtLink v-if="prev" :to="prev._path">{{ prev.title }}</NuxtLink>
        <NuxtLink v-if="next" :to="next._path">{{ next.title }}</NuxtLink>
      </div>
    </main>
  </div>
</template>

<style lang="scss" scoped>
.help {
  margin: auto;
  width: 100%;
  max-width: 1280px;
  padding: 0 30px;
  min-height: 100vh;
  display: flex;

  .sidebar {
    position: sticky;
    top: 0;
    width: 320px;
    padding: 0 1rem;
    height: 100vh;
    overflow: auto;

    .group-title {
      margin: 28px 0 12px;
      text-transform: capitalize;
    }

    a {
      color: inherit;
      text-decoration: none;
      padding: 0.5rem 1rem;
      border-left: 1px solid rgba(#111, 0.1);
      display: block;

      &.toc {
        padding-left: 2rem;
      }

      &.router-link-active {
        border-left: 1px solid rgba(#111, 0.4);
      }
    }
  }

  main {
    padding: 1rem;
    border-left: 1px solid rgba(#111, 0.1);
    flex-grow: 1;

    :deep(> *) {
      width: 100%;
      margin-right: auto;
      margin-left: auto;
      max-width: 768px;
    }

    :deep(h2) {
      margin: 0;
      font-weight: 700;
      font-size: 1.5em;
      margin-top: 2em;
      margin-bottom: 1em;
      line-height: 1.3333333;
      border-bottom: 1px solid rgba(#111, 0.1);
      padding-bottom: 4px;

      a {
        color: inherit;
        text-decoration: none;
      }
    }

    .paging {
      padding: 120px 0;
      justify-content: space-between;
      display: flex;
      a {
        padding: 1rem;
        border: 1px solid rgba(#111, 0.1);
      }
    }
  }
}
</style>
