<template>
  <ul>
    <li
      class="inline font-light text-[12px] leading-[17px] 2xl:text-[14px] 2xl:leading-[19px]"
      :style="{ color: color }"
      v-for="crumb in breadcrumbs"
      :key="crumb.name"
    >
      <nuxt-link :to="crumb.link">{{ crumb.name }}</nuxt-link>
    </li>
  </ul>
</template>

<script>
export default {
  props: ["breadcrumbs", "color"],
  head() {
    const structuredData = {
      "@context": "https://schema.org",
      "@type": "BreadcrumbList",
      itemListElement: []
    };
    this.breadcrumbs.forEach((crumb, index) => {
      structuredData.itemListElement.push({
        "@type": "ListItem",
        position: index + 1,
        name: crumb.name,
        item: `https://lolavanpraag.netlify.app${crumb.link}`
      });
    });

    return {
      script: [
        {
          type: "application/ld+json",
          json: structuredData
        }
      ]
    };
  }
};
</script>

<style scoped>
ul li + li:before {
  padding-left: 2px;
  color: black;
  content: "/\00a0";
}

.nuxt-link-exact-active {
  color: black;
}
</style>
