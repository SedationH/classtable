<template>
	<view class="table">
		<view class="table-time">
	        <view class="table-time-img"></view>
	        <view class="table-time-morning">上<br>午</view>
	        <view class="table-time-afternoon">下<br>午</view>
	        <view class="table-time-evening">晚<br>上</view>
        </view>
       <scroll-view class="table-course" scroll-x="true">
           <view class="day">
               <view class="head">周一</view>
               <view class="course"><m-item></m-item></view>
               <view class="course"><m-item></m-item></view>
               <view class="course"><m-item></m-item></view>
               <view class="course"><m-item></m-item></view>
               <view class="course"><m-item></m-item></view>
           </view>
           <view class="day">
               <view class="head">周二</view>
               <view class="course"><m-item></m-item></view>
               <view class="course"><m-item></m-item></view>
               <view class="course"><m-item></m-item></view>
               <view class="course"><m-item></m-item></view>
               <view class="course"><m-item></m-item></view>
           </view>
           <view class="day">
               <view class="head">周三</view>
               <view class="course"><m-item></m-item></view>
               <view class="course"><m-item></m-item></view>
               <view class="course"><m-item></m-item></view>
               <view class="course"><m-item></m-item></view>
               <view class="course"><m-item></m-item></view>
           </view>
           <view class="day">
               <view class="head">周四</view>
               <view class="course"><m-item></m-item></view>
               <view class="course"><m-item></m-item></view>
               <view class="course"><m-item></m-item></view>
               <view class="course"><m-item></m-item></view>
               <view class="course"><m-item></m-item></view>
           </view>
           <view class="day">
               <view class="head">周五</view>
               <view class="course"><m-item></m-item></view>
               <view class="course"><m-item></m-item></view>
               <view class="course"><m-item></m-item></view>
               <view class="course"><m-item></m-item></view>
               <view class="course"><m-item></m-item></view>
           </view>
           <view class="day">
               <view class="head">周六</view>
               <view class="course"><m-item></m-item></view>
               <view class="course"><m-item></m-item></view>
               <view class="course"><m-item></m-item></view>
               <view class="course"><m-item></m-item></view>
               <view class="course"><m-item></m-item></view>
           </view>
           <view class="day">
               <view class="head">周日</view>
               <view class="course"><m-item></m-item></view>
               <view class="course"><m-item></m-item></view>
               <view class="course"><m-item></m-item></view>
               <view class="course"><m-item></m-item></view>
               <view class="course"><m-item></m-item></view>
           </view>
       </scroll-view>
	</view>
</template>

<script>
    import item from '@/components/item.vue'
	export default {
		data() {
			return {
				
			};
		},
        components: {
            'm-item': item
        }
	}
</script>

<style scoped>
    view {
        margin: 0px;
        padding: 0px;
    }
    .table {
        height: 100%;
        width: 100%;
    }
    .table-time {
        position: fixed;
        top: 0;
        left: 0;
        width: 2rem;
        height: 100%;
        font-weight: 300;
        font-size: .8rem;        
    }
    .table-time-img {
        height: 47px;
        background: url('data:image/svg+xml;base64,PD94bWwgdmVyc2lvbj0iMS4wIiBzdGFuZGFsb25lPSJubyI/PjwhRE9DVFlQRSBzdmcgUFVCTElDICItLy9XM0MvL0RURCBTVkcgMS4xLy9FTiIgImh0dHA6Ly93d3cudzMub3JnL0dyYXBoaWNzL1NWRy8xLjEvRFREL3N2ZzExLmR0ZCI+PHN2ZyB0PSIxNTc5Mjc0NjU3ODEyIiBjbGFzcz0iaWNvbiIgdmlld0JveD0iMCAwIDEwMjQgMTAyNCIgdmVyc2lvbj0iMS4xIiB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHAtaWQ9IjQ1MjQiIHhtbG5zOnhsaW5rPSJodHRwOi8vd3d3LnczLm9yZy8xOTk5L3hsaW5rIiB3aWR0aD0iMjAwIiBoZWlnaHQ9IjIwMCI+PGRlZnM+PHN0eWxlIHR5cGU9InRleHQvY3NzIj48L3N0eWxlPjwvZGVmcz48cGF0aCBkPSJNNDU1LjI2IDg3Mi41MmMtMTE2LjE2IDAtMjMzLjE0LTguMzktMzQ3LjcxLTI0Ljk0YTY2LjQzIDY2LjQzIDAgMCAxLTQwLjU2LTIyLjA2IDY1LjgzMiA2NS44MzIgMCAwIDEtMTYuMjMtNDMuMjd2LTU2Ny41YzAtMzUuOTUgMjkuNC02NS4yIDY1LjU0LTY1LjJoNjgzLjUxYzM2LjE0IDAgNjUuNTQgMjkuMjUgNjUuNTQgNjUuMnY1NjcuMzhjMCAzMi42OC0yNC41MiA2MC43OC01Ny4wMyA2NS4zNi0xMTcuNCAxNi41NC0yMzUuNjYgMjQuOTYtMzUxLjUgMjUuMDNoLTEuNTZ6TTExNi4zIDIwOS41NGMtMy4wNSAwLTUuNTQgMi4zMy01LjU0IDUuMnY1NjcuNWMwIDIuOTUgMi4zMSA1LjUgNS4zNyA1Ljk0IDExMS43MSAxNi4xNCAyMjUuMDMgMjQuMjEgMzM5LjExIDI0LjIxIDExNC4zOSAwIDIyOS41NC04LjExIDM0NC43MS0yNC4zMyAzLjA4LTAuNDMgNS40LTIuOTkgNS40LTUuOTVWMjE0Ljc0YzAtMi44Ny0yLjQ4LTUuMi01LjU0LTUuMkgxMTYuM3oiIGZpbGw9IiMzNTJFNzAiIHAtaWQ9IjQ1MjUiPjwvcGF0aD48cGF0aCBkPSJNMjc5LjIyIDI3My43MWMtMTYuNTcgMC0zMC0xMy40My0zMC0zMFY4NS45MWMwLTE2LjU3IDEzLjQzLTMwIDMwLTMwczMwIDEzLjQzIDMwIDMwdjE1Ny44YzAgMTYuNTctMTMuNDQgMzAtMzAgMzB6TTYzNi45IDI3My43MWMtMTYuNTcgMC0zMC0xMy40My0zMC0zMFY4NS45MWMwLTE2LjU3IDEzLjQzLTMwIDMwLTMwczMwIDEzLjQzIDMwIDMwdjE1Ny44YzAgMTYuNTctMTMuNDQgMzAtMzAgMzB6TTc0NC42NiA0MDEuNTVIMTcxLjQ1Yy0xNi41NyAwLTMwLTEzLjQzLTMwLTMwczEzLjQzLTMwIDMwLTMwaDU3My4yMWMxNi41NyAwIDMwIDEzLjQzIDMwIDMwcy0xMy40MyAzMC0zMCAzMHoiIGZpbGw9IiMzNTJFNzAiIHAtaWQ9IjQ1MjYiPjwvcGF0aD48cGF0aCBkPSJNNDA2Ljc4IDczOS41NGMtNy42NyAwLTE1LjM0LTIuOTItMjEuMi04Ljc3TDI2Ni4zNiA2MTEuNzFjLTExLjcyLTExLjcxLTExLjc0LTMwLjctMC4wMy00Mi40MyAxMS43MS0xMS43MiAzMC43LTExLjc0IDQyLjQzLTAuMDNsOTggOTcuODZMNjIzLjI3IDQ1MC40YzExLjcxLTExLjcyIDMwLjcxLTExLjczIDQyLjQzLTAuMDJzMTEuNzMgMzAuNzEgMC4wMiA0Mi40M2wtMjM3LjcgMjM3LjkzYy01Ljg3IDUuODctMTMuNTUgOC44LTIxLjI0IDguOHoiIGZpbGw9IiNGRjk2NjgiIHAtaWQ9IjQ1MjciPjwvcGF0aD48cGF0aCBkPSJNNDYzLjQzIDk2OGMtOTkuNzEgMC0xOTguODUtNC44My0yOTYuOTYtMTQuNDktMTYuNDktMS42Mi0yOC41NC0xNi4zMS0yNi45Mi0zMi44IDEuNjItMTYuNDkgMTYuMzEtMjguNTQgMzIuOC0yNi45MiAyMjAuOSAyMS43NSA0NDcuMzUgMTguNSA2NzMuMDYtOS42NyAzOC42Ny00LjgzIDY3Ljg0LTM3LjkyIDY3Ljg0LTc2Ljk3di01MzMuNmMwLTE2LjU3IDEzLjQzLTMwIDMwLTMwczMwIDEzLjQzIDMwIDMwdjUzMy42MmMwIDY5LjI1LTUxLjc2IDEyNy45NC0xMjAuNDEgMTM2LjVDNzIyLjkxIDk1OS44OSA1OTIuNzEgOTY4IDQ2My40MyA5Njh6IiBmaWxsPSIjRkY0RTgzIiBwLWlkPSI0NTI4Ij48L3BhdGg+PC9zdmc+') no-repeat center;
        background-size: 20px 20px;
        position: relative;
    }
    .table-time-morning,
    .table-time-afternoon {
        height: calc(40% - 18.8px);
    }
    .table-time-evening {
        height: calc(20% - 9.4px);
    }
    .table-time > view {
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
    }
   .table-course {
        position: absolute;
        top: 0;
        left: 2rem;
        height: 100%;
        width: calc(100% - 2rem);
        white-space: nowrap;
        font-size: .8rem;
    }
    .day {
        display: inline-block;
        width: 20%;
        height: 100vh;
    }     
    .head {
        border-bottom: 1px solid rgb(230,230,230);
        height: 47px;
        line-height: 47px;
        width: 100%;
        text-align: center;
    }
    .course {
        width: 100%;
        height: calc(20% - 9.4px);
    }
</style>

        