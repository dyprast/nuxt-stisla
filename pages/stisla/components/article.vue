<template>
  <div>
    <ComponentsArticle />
  </div>
</template>

<script>
import ComponentsArticle from "@/components/pages/ComponentsArticle";
export default {
  head: {
    title: "Components - Article - Nuxt Stisla",
  },
  components: {
    ComponentsArticle,
  },
  mounted(){
		this.$store.commit("INITIAL_PAGE", { page: "components-article" })
	}
};
</script>

<style scoped>
</style>