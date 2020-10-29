<template>
  <div>
    <ComponentsChatBox />
  </div>
</template>

<script>
import ComponentsChatBox from "@/components/pages/ComponentsChatBox";
export default {
  head: {
    title: "Components - Chat Box - Nuxt Stisla",
    script: [
      { src: "/js/page/components-chat-box.js", body: true },
    ],
  },
  components: {
    ComponentsChatBox,
  },
  mounted(){
		this.$store.commit("INITIAL_PAGE", { page: "components-chatBox" })
	}
};
</script>

<style scoped>
</style>