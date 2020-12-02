<template>
	<view class="uni-popup-share">
		<view class="uni-share-content">
			<view style="flex-direction:row;margin-left: 30rpx;margin-top: 10rpx;">
				<view style="width: 30%;">
					<image style="width: 100%;height: 200rpx;" src="../../static/shop/item3.jpg" mode="scaleToFill"></image>
				</view>
				<view style="width: 70%;margin-left: 8rpx;">
					<view style="height: 30%;"/>
					<text style="color: #74bb7a; font-size: 40rpx;">￥20</text>
					<view style="height: 95rpx;">
						<text class="topic_cont_text">{{"已选择 主香调：雨后新竹香气；下单后3-5天发出，近期配送时效延长。"}}</text>
					</view>
				</view>
			</view>
			<view class="link-top"></view>
			<view style="margin-left: 30rpx;margin-top: 20rpx;">
				<text style="color: #000000; font-weight:550;font-size: 36rpx;">商品属性</text>
				<view style="margin-top: 20rpx; background-color: #f1f8f1; width: 350rpx; height: 70rpx;flex-direction:inherit;align-items: center;">
					<text style="color: #3fb83f;font-size: 30rpx;margin-top: 14rpx;">主香调：雨后新竹香气</text>
				</view>
			</view>
			<view class="link-top"></view>
			<view style="margin-left: 30rpx;margin-top: 20rpx;">
				<text style="color: #000000; font-weight:550;font-size: 36rpx;">发货时效</text>
				<view style="margin-top: 20rpx; background-color: #f1f8f1; width: 570rpx; height: 70rpx;flex-direction:inherit;align-items: center;">
					<text style="color: #3fb83f;font-size: 30rpx;margin-top: 14rpx;">下单后3-5天发出，近期配送时效延长。</text>
				</view>
			</view>
			<view class="link-top"></view>
			<view style="margin-left: 30rpx;margin-right: 30rpx;flex-direction: row;height: 100rpx;">
				<view style="width: 45%;height: 100%;flex-direction: row;align-items: center;">
					<text style="color: #000000; font-weight:550;font-size: 36rpx;">购买数量</text>
				</view>
			
				<view style="width: 55%;height: 100%;flex-direction: row;align-items: center;">
					<text style="color: #3fb83f;font-size: 30rpx;">每人限购5件</text>
					<view style="margin-left: 15rpx;border-radius: 10rpx;width: 60rpx;height: 60rpx;background-color: #f2f3f5;flex-direction: inherit;">
						<view class="line-jian"/>
					</view>
					<view style="margin-left: 5rpx;width: 60rpx;height: 60rpx;background-color: #f2f3f5;flex-direction: inherit;">
						<view style="flex-direction: inherit;width: 40%;margin-left: 35%;">
							<text style="color: #909090;align-self: center;">5</text>
						</view>
					</view>
					<view style="margin-left: 5rpx;border-radius: 10rpx;width: 60rpx;height: 60rpx;background-color: #f2f3f5;flex-direction: inherit;">
						<view style="flex-direction: inherit;width: 40%;margin-left: 30%">
							<text style="color: #000000;align-self: center;">+</text>
						</view>
					</view>
				</view>
			</view>
			<view style="height: 30px"/>
			<view style="height: 10%;flex-direction: row;"> 
				<view style="width: 50%;height: 100rpx;">
					<image style="width: 95%;height: 100%;align-self: flex-end;" src="../../static/buy/add.png"/>
				</view>
				<view style="width: 50%;height: 100rpx;">
					<image style="width: 95%;height: 100%;align-self: flex-start;" src="../../static/buy/buy.png"/>
				</view>
			</view>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
			}
		},
		methods: {
			/**
			 * 关闭窗口
			 */
			close() {
				this.popup.close()
			}
		}
	}
</script>
<style scoped>
	.uni-icons {
		font-family: uniicons;
		text-decoration: none;
		text-align: center;
	}
	
	.uni-popup-share {
		background-color: #fff;
		border-radius: 15px 15px 0px 0px;
	}
	
	.uni-share-content {
		/* #ifndef APP-NVUE */
		display: flex;
		/* #endif */
		flex-direction: column;
		justify-content: center;
		padding-top: 10px;
	}

	.uni-share-content-box {
		/* #ifndef APP-NVUE */
		display: flex;
		/* #endif */
		flex-direction: row;
		flex-wrap: wrap;
		width: 360px;
	}

	.uni-share-content-item {
		width: 90px;
		/* #ifndef APP-NVUE */
		display: flex;
		/* #endif */
		flex-direction: column;
		justify-content: center;
		padding: 10px 0;
		align-items: center;
	}

	.uni-share-content-item:active {
		background-color: #f5f5f5;
	}

	.uni-share-image {
		width: 30px;
		height: 30px;
	}

	.uni-share-text {
		margin-top: 10px;
		font-size: 14px;
		color: #3B4144;
	}

	.uni-share-button-box {
		/* #ifndef APP-NVUE */
		display: flex;
		/* #endif */
		flex-direction: row;
		padding: 10px 15px;
	}

	.uni-share-button {
		flex: 1;
		border-radius: 50px;
		color: #666;
		font-size: 16px;
	}

	.uni-share-button::after {
		border-radius: 50px;
	}
	
	.topic_cont_text{
		padding: 10upx;
		overflow: hidden;
		word-break: break-all;  /* break-all(允许在单词内换行。) */
		text-overflow: ellipsis;  /* 超出部分省略号 */
		display: -webkit-box; /** 对象作为伸缩盒子模型显示 **/
		-webkit-box-orient: vertical; /** 设置或检索伸缩盒对象的子元素的排列方式 **/
		-webkit-line-clamp: 2; /** 显示的行数 **/
		color: #8b8b8b;
		font-size: 28rpx;
	}
	
	.link-top {
		margin-top: 20rpx;
		width: 94%;
		height: 1px;
		border-top: solid #f4f4f4 1px;
		align-self: center;
	}
	
	.line-jian {
		width: 50%;
		height: 1px;
		border-top: solid #909090 1px;
		align-self: center;
		margin-left: 25%;
	}
</style>