## 使用方法

index.vue
<code>

	<template>
		<Datepicker v-ref:datepicker></Datepicker>
	</template>

	<script>
		import Datepicker from 'path/Datepicker'

		export default  {
			data () {
				return {

				}
			},
			components: { 'Datepicker': Datepicker },
			method:{

			},

			created:{
				var newdate = new Date();
				this.$refs.datepicker.selectdate = newdate.getFullYear()+'-'+(newdate.getMonth()+1)+'-'+newdate.getDate();
			}
		}
	</script>
</code>

## 依赖的库或者组件

<ul>
	<li>1、vuejs</li>
	<li>2、bootstrap</li>
</ul>

## 图

![](http://7xioxc.com1.z0.glb.clouddn.com/github/vc1.jpg)
![](http://7xioxc.com1.z0.glb.clouddn.com/github/vc2.jpg)
![](http://7xioxc.com1.z0.glb.clouddn.com/github/vc3.jpg)