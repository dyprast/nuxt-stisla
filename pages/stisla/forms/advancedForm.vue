<template>
  <div>
    <AdvancedForm />
  </div>
</template>

<script>
import AdvancedForm from "@/components/pages/FormsAdvancedForm";
export default {
  head: {
    title: "Forms - Advanced Form - Nuxt Stisla",
    link: [
      { rel: "stylesheet", href: "/modules/bootstrap-daterangepicker/daterangepicker.css" },
      { rel: "stylesheet", href: "/modules/bootstrap-colorpicker/dist/css/bootstrap-colorpicker.min.css" },
      { rel: "stylesheet", href: "/modules/select2/dist/css/select2.min.css" },
      { rel: "stylesheet", href: "/modules/jquery-selectric/selectric.css" },
      { rel: "stylesheet", href: "/modules/bootstrap-timepicker/css/bootstrap-timepicker.min.css" },
      { rel: "stylesheet", href: "/modules/bootstrap-tagsinput/dist/bootstrap-tagsinput.css" },
    ],
    script: [
      { src: "/modules/cleave-js/dist/cleave.min.js" },
			{ src: "/modules/cleave-js/dist/addons/cleave-phone.us.js" },
			{ src: "/modules/jquery-pwstrength/jquery.pwstrength.min.js" },
			{ src: "/modules/bootstrap-daterangepicker/daterangepicker.js" },
			{ src: "/modules/bootstrap-colorpicker/dist/js/bootstrap-colorpicker.min.js" },
			{ src: "/modules/bootstrap-timepicker/js/bootstrap-timepicker.min.js" },
			{ src: "/modules/bootstrap-tagsinput/dist/bootstrap-tagsinput.min.js" },
			{ src: "/modules/select2/dist/js/select2.full.min.js" },
			{ src: "/modules/jquery-selectric/jquery.selectric.min.js" },

			{ src: "/js/page/forms-advanced-forms.js", body: true }
    ],
  },
  components: {
    AdvancedForm,
  },
  mounted(){
		this.$store.commit("INITIAL_PAGE", { page: "forms-advancedForm" })
	}
};
</script>

<style scoped>
</style>