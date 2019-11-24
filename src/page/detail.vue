<template>
	<div class="detail-page">
		<div class="video">
			<video src="http://v3.mukewang.com/shizhan/59f8498ae420e5be578b459b/H.mp4" controls="controls"></video>
			<router-link to="/">
				<div class="video-back"><</div>
			</router-link>
		</div>
	</div>
</template>
<style scoped>
	.video{
		position: relative;
		height: 3.82rem;
	}
	.video video{
		width: 100%;
		height: 100%;
	}
	.video-back{
		position: absolute;
		top: 21px;
		left: 16px;
		text-align: center;
		color: #fff;
		font-size: 18px;
		line-height: 32px;
		border-radius: 3px;
		width: 32px;
		height: 32px;
		background: rgba(0,0,0,.5);
	}
</style>