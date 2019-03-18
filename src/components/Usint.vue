<template>
	<div>
		<h2>添加博客</h2>
		<form>
			<label>博客标题：</label>
			<input type="text" v-model="blog.title" required />
			<label>博客内容</label>
			<textarea v-model="blog.content"></textarea>
		</form>
		<hr>
		<div id="previewe">
			<h3>博客总览</h3>
			<p>博客标题：{{blog.title}}</p>
			<p>博客内容:</p>
			<p>{{blog.content}}</p>
		</div>
	</div>
</template>
<script type="text/javascript">
export default {
	name:"usint",
	data(){
		return{
		blog:{
			title:"",
			content:""
		}
	}
	}
}
</script>