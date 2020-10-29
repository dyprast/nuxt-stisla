<template>
  <div>
    <ComponentsUser />
  </div>
</template>

<script>
import ComponentsUser from "@/components/pages/ComponentsUser";
export default {
  head: {
    title: "Components - User - Nuxt Stisla"
	},
  components: {
    ComponentsUser,
  },
  mounted(){
		this.$store.commit("INITIAL_PAGE", { page: "components-user" })
	}
};
</script>

<style scoped>
</style>