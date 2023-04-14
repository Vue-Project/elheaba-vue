<template>
	<section class="common-section bg-gray">
		<header class="section-header">
			<div class="container">
				<span>Our Blog</span>
				<h2>Latest News</h2>
			</div>
		</header>
		<div class="container">
			<div class="row">

				<div class="col-md-4" v-for='service in services' :key="service.id">
					<div class="post-item">
						<figure class="post-thumb">
							<!-- <img src="~/assets/images/posts/post-01.png" alt="Work 1" > -->
						</figure>
						<h4>What is Lorem Ipsum?</h4>
						<p>Lorem Ipsum is simply dummy text of the printing and typesetting industry.</p>
					</div>
				</div>

			</div>
		</div>
	</section>
</template>

<script>
export default {
	data() {
    return {
			services:[
				{
					id: 0,
					icon: '~/assets/images/posts/post-01.png',
					name: 'What is Lorem Ipsum?',
					text: 'Lorem Ipsum is simply dummy text of the printing and typesetting industry.'
				},
	
			]
		}
				
	}

}
</script>

<style>

</style>