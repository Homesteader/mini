<template name = "page-head">
	<view class= "uni-page-head">
		<view class="uni-page-head-title">{{title}}</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				name: "page-head",
				props: {
					title: {
						type: String,
						default: ""
					}
				}
			}
		}
	}
</script>
