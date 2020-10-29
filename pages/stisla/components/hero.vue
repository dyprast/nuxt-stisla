<template>
  <div>
    <ComponentsHero />
  </div>
</template>

<script>
import ComponentsHero from "@/components/pages/ComponentsHero";
export default {
  head: {
    title: "Components - Hero - Nuxt Stisla",
  },
  components: {
    ComponentsHero,
  },
  mounted(){
		this.$store.commit("INITIAL_PAGE", { page: "components-hero" })
	}
};
</script>

<style scoped>
</style>