<template>
  <div>
    <ComponentsTable />
  </div>
</template>

<script>
import ComponentsTable from "@/components/pages/ComponentsTable";
export default {
  head: {
    title: "Components - Table - Nuxt Stisla",
    script: [
      { src: "/modules/jquery-ui/jquery-ui.min.js" },
      { src: "/js/page/components-table.js" },
    ],
  },
  components: {
    ComponentsTable,
  },
  mounted(){
		this.$store.commit("INITIAL_PAGE", { page: "components-table" })
	}
};
</script>

<style scoped>
</style>