<template>
	<header>
	  <nav class="navbar is-light" role="navigation" aria-label="main navigation">
	    <div class="container">
	        <div class="navbar-start">
	          <h1 class="title navbar-item">
	            foutlook
	          </h1>
	        </div>
	        <div class="navbar-end navbar-item">
	          <p>設定</p>
	        </div>
	    </div>
	  </nav>
	  <nav class="breadcrumb has-succeeds-separator" aria-label="breadcrumbs">
			<div class="container">
				<ul class="navbar-item" v-if="city_name != null">
				    <li>
				    	<nuxt-link to="/">HOME</nuxt-link>
				    </li>
				    <li class="is-active">
				    	<a :href="city_url" aria-current="page">{{city_name}}の天気情報</a>
				    </li>
			  	</ul>
			</div>
		</nav>
	</header>
</template>

<script>
export default {
	name: 'Header',
	props: {
		city_name: String,
		city_url: String
	}
}
</script>

<style scoped>

</style>