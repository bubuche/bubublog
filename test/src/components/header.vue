<template>
	<div class="row header">
		<div class="col-lg-4">
			<a href="#" class="pull-right">
				<img src="./src/logo.jpg" alt="logojpg" class="img-responsive center-block logo">
			</a>
		</div>
		<div class="col-lg-7 col-lg-offset-1">
			<ul class="nav nav-pills nav-list center">
				<li class="nav-list-item {{active? active : ''}}" v-for="item in title">
					<a href={{item.address}}>{{item.name}}</a>
				</li>
			</ul>
		</div>
		<!-- <button v-on:click="modify()">add</button> -->
	</div>	
</template>
<script>
  	export default {
		data () {
			return {
				title: [
					{
						name: 'BLOG',
						address: './index.html',
						active: true
					},
					{
						name: 'ARCHIVE',
						address: './archive.html',
						active: false
					},
					{
						name: 'ABOUT',
						address: './about.html',
						active: false
					},
					{
						name: 'RESUME',
						address: '#',
						active: false
					}
				]
			}
		},
		// methods: {
		// 	modify() {
		// 		this.title[0].name = 'bangbang';
		// 	}
		// }
	}
</script>
<style>
	.header{
		padding: 50px 0;
	}
	.logo{
		width:60px;
		height:60px;
		line-height:60px;
	}
</style>