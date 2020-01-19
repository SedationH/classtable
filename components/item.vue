<template>
	<view class="item">
		    <text>课程信息</text>
		    <text>A509</text>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				
			};
		}
	}
</script>

<style>
    .item {
        display: flex;
        flex-direction: column;
        height: calc(100% - 8px);
        width: calc(100% - 8px);
        padding: 2px;
        margin-bottom: 2px;
        margin-right: 4px;
        border-radius: 5px;
        font-size: 0.6rem;
        font-weight: 300;
        word-break: break-all;
        white-space: normal;
        justify-content: space-between;
        background-color: #e6e5e8;
        text-align: start;
    }
    .item view {
        width: 100%;
    }
    .room {
        position: relative;
        bottom: 0px;
    }
</style>
