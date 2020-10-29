<template>
  <div>
    <ComponentsPricing />
  </div>
</template>

<script>
import ComponentsPricing from "@/components/pages/ComponentsPricing";
export default {
  head: {
    title: "Components - Pricing - Nuxt Stisla",
  },
  components: {
    ComponentsPricing,
  },
  mounted(){
		this.$store.commit("INITIAL_PAGE", { page: "components-pricing" })
	}
};
</script>

<style scoped>
</style>