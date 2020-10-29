<template>
  <div>
    <ComponentsTab />
  </div>
</template>

<script>
import ComponentsTab from "@/components/pages/ComponentsTab";
export default {
  head: {
    title: "Components - Tab - Nuxt Stisla",
  },
  components: {
    ComponentsTab,
  },
  mounted(){
		this.$store.commit("INITIAL_PAGE", { page: "components-tab" })
	}
};
</script>

<style scoped>
</style>