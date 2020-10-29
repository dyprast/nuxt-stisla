<template>
  <div>
    <ComponentsEmptyState />
  </div>
</template>

<script>
import ComponentsEmptyState from "@/components/pages/ComponentsEmptyState";
export default {
  head: {
    title: "Components - Empty State - Nuxt Stisla",
  },
  components: {
    ComponentsEmptyState,
  },
  mounted(){
		this.$store.commit("INITIAL_PAGE", { page: "components-emptyState" })
	}
};
</script>

<style scoped>
</style>