<template>
	<div class="row col-lg-8 col-lg-offset-2">
		<ul class="nav nav-pills nav-list center">
			<li class="nav-list-item" v-for="item in passage">
				<h2>{{item.title}}</h2>
				<small>{{item.date}}</small>
				<div>{{item.content}}</div>
			</li>
		</ul>
	</div>
</template>
<script>
	export default{
		data(){
			return{
				title
			}
		}
	}
</script>