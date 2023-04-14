<template>
	<section class="common-section services services-05 bg-gray">
			<div class="container">
					<div class="row">
							<div class="col-md-5">
									<h1>Services We Provide</h1>
									<p>We deploy processes and services that show high value, immediate and lasting impact on their business performance.</p>
							</div>

							<div class="col-md-7">
									<div class="row">
											<div class="col-md-6" v-for='service in services.slice(0,3)' :key="service.id">
													<div class="service-item">
															<figure class="service-icon">
																	<img :src="getImgUrl(service.icon)" :alt="service.name">
															</figure>
															<h2>{{service.name}}</h2>
															<p>{{service.desc}}</p>
													</div>
											</div>
						
									</div>
							</div>

					</div>

			</div>
	</section>
</template>

<script>
// export default {
// 		data() {
//     return {
// 			services:[
// 				{
// 					id: 0,
// 					icon: 'services/service-01.png',
// 					name: 'Branding',
// 					desc: 'Lorem Ipsum is simply dummy text of the printing and typesetting industry.'
// 				},
// 				{
// 					id: 1,
// 					icon: 'services/service-02.png',
// 					name: 'UI & UX',
// 					desc: 'Lorem Ipsum is simply dummy text of the printing and typesetting industry.'
// 				},
// 				{
// 					id: 2,
// 					icon: 'services/service-03.png',
// 					name: 'Web App',
// 					desc: 'Lorem Ipsum is simply dummy text of the printing and typesetting industry.'
// 				},
// 				{
// 					id: 3,
// 					icon: 'services/service-04.png',
// 					name: 'Mob App',
// 					desc: 'Lorem Ipsum is simply dummy text of the printing and typesetting industry.'
// 				},
// 				{
// 					id: 4,
// 					icon: 'services/service-05.png',
// 					name: 'Markting',
// 					desc: 'Lorem Ipsum is simply dummy text of the printing and typesetting industry.'
// 				},
// 				{
// 					id: 5,
// 					icon: 'services/service-06.png',
// 					name: 'Support',
// 					desc: 'Lorem Ipsum is simply dummy text of the printing and typesetting industry.'
// 				},


	
// 			]
// 		}
// 	},
// 	methods:{
// 		getImgUrl: function (imagePath) {
//       return require('@/assets/images/' + imagePath);
//     }
// 	}


// }
</script>

<style>

</style>