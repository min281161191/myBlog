<template>
  <nav class="navigation-bar container-fluid">
    <div class="row">
    	<div class="col-md-2 logo"><img class="img" src="../assets/user.jpg" alt="logo"> 星孑</div>
    	<div class="col-md-3 share">
    		<span>分享</span>
    		<a href="#" class="share-weixin"><i class="fa fa-weixin"></i></a>
    		<a href="#" class="share-qq"><i class="fa fa-qq"></i></a>
    		<a href="#" class="share-weibo"><i class="fa fa-weibo"></i></a>
    	</div>
    	<div class="col-md-7 classes text-right">
    		<span><a href="#">原创心得</a></span>
    		<span><a href="#">转载博文</a></span>
    		<span><a href="#">干货链接</a></span>
    	</div>
    </div>
  </nav>
</template>

<script>
export default {
  data () {
    return {
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
	/*导航容器*/
	.container-fluid {
		height: 80px;
		background: #333538;
	}
	.container-fluid > div {
		max-width:1520px;
		margin: auto; 
		line-height: 80px;
		color: #f0f9ff;
	}
	/*logo*/
	.logo{
		font-size: 3rem;
		cursor: pointer;
	}
	.logo img {
		width: 3.5rem;
		height: 3.5rem;
		border-radius: 50%;
	}
	/*分享*/
	.share span{
		padding-right: 10px;
		font-size: 2.8rem;
		color: #afafaf;
	}
	.share a {
		padding-right: 10px;
		font-size: 3rem;
		color: #aaafb9;		
	}
	.share-weixin:hover{
		color: #62b900;
	}
	.share-qq:hover{
		color: #428bca;
	}
	.share-weibo:hover{
		color: #d9534f;
	}
	/*类别*/
	.classes span {
		padding: 0 10px;
	}
	.classes span + span{
		border-left: 1px solid #ccc;
	}
	.classes *{
		font-size: 2rem;
		color: #aaafb9;
	}
	.classes *:hover {
		color: #fff;
	}
	.classes a:hover {
		text-decoration: none;
	}
</style>
