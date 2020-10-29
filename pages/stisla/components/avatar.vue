<template>
  <div>
    <ComponentsAvatar />
  </div>
</template>

<script>
import ComponentsAvatar from "@/components/pages/ComponentsAvatar";
export default {
  head: {
    title: "Components - Avatar - Nuxt Stisla",
  },
  components: {
    ComponentsAvatar,
  },
  mounted(){
		this.$store.commit("INITIAL_PAGE", { page: "components-avatar" })
	}
};
</script>

<style scoped>
</style>