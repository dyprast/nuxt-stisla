<template>
  <div>
    <ComponentsWizard />
  </div>
</template>

<script>
import ComponentsWizard from "@/components/pages/ComponentsWizard";
export default {
  head: {
    title: "Components - Wizard - Nuxt Stisla",
  },
  components: {
    ComponentsWizard,
  },
  mounted(){
		this.$store.commit("INITIAL_PAGE", { page: "components-wizard" })
	}
};
</script>

<style scoped>
</style>