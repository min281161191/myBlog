<template>
	<section class="container-fluid">
		<div class="row">
			<div class="col-md-9 article">
				<div class="row title-border"><i class="fa fa-chevron-right"></i>新货</div>
				<div class="row" v-for="msg in newLists">
					<div class="col-md-7 col-md-offset-1"><a href="#" v-text="msg.name"></a></div>
					<div class="col-md-2"><span href="#" v-text="msg.creationTime"></span></div>
					<div class="col-md-2"><span href="#" v-text="msg.author"></span></div>
				</div>
				<div class="row title-border"><i class="fa fa-chevron-right"></i>好货</div>
				<div class="row" v-for="msg in hotLists">
					<div class="col-md-7 col-md-offset-1"><a href="#" v-text="msg.name"></a></div>
					<div class="col-md-2"><span href="#" v-text="msg.creationTime"></span></div>
					<div class="col-md-2"><span href="#" v-text="msg.author"></span></div>
				</div>
				<div class="row title-border"><i class="fa fa-chevron-right"></i>山途</div>
				<div class="row"></div>	
			</div>
			<div class="col-md-3"></div>
		</div>
	</section>
</template>
<script>
	export default {
	  data () {
	    return {
	    	newLists:[
	    		{name:'test1',creationTime:'2016-05-06',author:'xingjie'},
	    		{name:'test2',creationTime:'2016-06-06',author:'xingjie'},
	    		{name:'test3',creationTime:'2016-07-06',author:'xingjie'}
	    	],
	    	hotLists:[
	    		{name:'test4',creationTime:'2016-08-06',author:'xingjie'},
	    		{name:'test5',creationTime:'2016-09-06',author:'xingjie'},
	    		{name:'test3',creationTime:'2016-07-06',author:'xingjie'}
	    	]
	    }
	  }
	}
</script>
<style scoped>
	section {
		min-height: 900px;	
		background: url(../assets/bg-image.jpg) no-repeat;
		background-size: cover;
	} 
	section > div.row {
		max-width: 1520px;
		margin: auto;
		background: #fff;
	}
	.article {
		padding-left: 30px;
		padding-right: 30px;
	}
	.article .fa {
		padding-right: 20px;
	}
	.title-border {
		margin: 20px;
		font-size: 2.5rem;
		line-height: 4rem;
		color: #fa5;
		border-bottom: 1px solid #fb6;
	}
</style>