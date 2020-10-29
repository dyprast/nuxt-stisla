<template>
  <div>
    <ComponentsMultipleUpload />
  </div>
</template>

<script>
import ComponentsMultipleUpload from "@/components/pages/ComponentsMultipleUpload";
export default {
  head: {
    title: "Components - Multiple Upload - Nuxt Stisla",
    link: [
      { rel: "stylesheet", href: "/modules/dropzonejs/dropzone.css" }
    ],
    script: [
      { src: "/modules/dropzonejs/min/dropzone.min.js" },
      { src: "/js/page/components-multiple-upload.js", body: true }
    ],
  },
  components: {
    ComponentsMultipleUpload,
  },
  mounted(){
		this.$store.commit("INITIAL_PAGE", { page: "components-multipleUpload" })
	}
};
</script>

<style scoped>
</style>