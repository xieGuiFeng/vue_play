<template>
  <div>
	<router-view></router-view>  
	<ul class="footer">
		<li class="icons">
			<router-link :to="{name: 'list'}">新闻列表</router-link>
		</li>
		<li class="icons">
			<router-link :to="{name: 'user'}">个人中心</router-link>
		</li>
	</ul>
  </div>
</template>

<script>
// @ is an alias to /src
// import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'Home',
  components: {
    // HelloWorld
  }
}
</script>

<style scoped lang="scss">
	li{
		list-style: none;
	}
	.footer{
		position: fixed;
		bottom: 0;
		left: 0;
		width: 100%;
		height: 60px;
		line-height: 60px;
		display: flex;
		flex-flow: row nowrap;
		justify-content: space-around;
	}
	.icons{
		font-size: 16px;
		flex: 1;
		text-align: center;
		border-top: 1px solid #42B983;
		a{
			color: #42B983;
			display: block;
			&.active{
				color: #fff;
				background-color: #42B983;
			}
		}
	}
	
</style>