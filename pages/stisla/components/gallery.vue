<template>
  <div>
    <ComponentsGallery />
  </div>
</template>

<script>
import ComponentsGallery from "@/components/pages/ComponentsGallery";
export default {
  head: {
    title: "Components - Gallery - Nuxt Stisla",
    link: [
      { rel: "stylesheet", href: "/modules/chocolat/dist/css/chocolat.css" }
    ],
    script: [
      { src: "/modules/chocolat/dist/js/jquery.chocolat.min.js" }
    ],
  },
  components: {
    ComponentsGallery,
  },
  mounted(){
		this.$store.commit("INITIAL_PAGE", { page: "components-gallery" })
	}
};
</script>

<style scoped>
</style>