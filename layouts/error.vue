<template>
	<div>
		<div class="section-header">
			<h1>Error Page</h1>
		</div>
		<div class="container mt-5">
			<div v-if="error.statusCode === 403" class="page-error">
				<div class="page-inner">
					<h1>403</h1>
					<div class="page-description">You do not have access to this page.</div>
				</div>
			</div>
			<div v-if="error.statusCode === 404" class="page-error">
				<div class="page-inner">
					<h1>404</h1>
					<div class="page-description">The page you were looking for could not be found.</div>
				</div>
			</div>
			<div v-if="error.statusCode === 500" class="page-error">
				<div class="page-inner">
					<h1>500</h1>
					<div class="page-description">Whoopps, something went wrong.</div>
				</div>
			</div>
			<div v-if="error.statusCode === 503" class="page-error">
				<div class="page-inner">
					<h1>503</h1>
					<div class="page-description">Be right back.</div>
				</div>
			</div>
		</div>
	</div>
</template>

<script>
export default {
  props: ["error"],
};
</script>