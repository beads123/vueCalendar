使用方法

====

index.vue

<code type="html">

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


===
依赖的库或者组件
<ul>
	<li>1、vuejs</li>
	<li>2、bootstrap</li>
</ul>