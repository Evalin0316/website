<template>
<div>
    <div class="item">
 		<div class="pic">
 			<img src="../assets/image/sign.png" alt="">
 		</div>
 		<div class="text">
 			<h2>點點簽</h2>
 			<p>「產品介紹」或是「關於我」常用的交錯漂浮版，一定要學起來! 好像會使用到絕對定位還是相對定位，一定要使用 Flex，新學了 flex-shrink。</p>
 		</div>
 	</div>

 	<!-- item02 -->
 	<div class="item">
 		<div class="text">
 			<h2>新手一定要寫註解</h2>
 			<p>不然一堆一樣的東西，回過頭來維護或寫到一半都會忘記為什麼會這樣...所以加註解非常重要，不要覺得自己記憶力很強啊!其實都很不管用的！</p>
 		</div>
 		<div class="pic">
 			<img src="https://picsum.photos/600/350?random=20" alt="">
 		</div>

 	</div>

 	<!-- item03 -->
 	<div class="item">
 		<div class="pic">
 			<img src="https://picsum.photos/600/350?random=30" alt="">
 		</div>
 		<div class="text">
 			<h2>有點難又不會太難</h2>
 			<p>區塊尺寸怎麼算、 Box-sizing 是甚麼、 CSS relative 相對定位、 網頁的色彩原理、 flex-direction 的原理、 「>」子代選取器、:nth-child(n) 選取器教學</p>
 		</div>
 	</div>

 	<!-- item04 -->
 	<div class="item">
 		<div class="text">
 			<h2>:nth-child(n) 選取器</h2>
 			<p>CSS3 新增的選取器，一定要學會，好厲害啊!! 只要架構清楚都不用再寫 class 來綁定跟套用效果啦! HTML 標籤變得好乾淨! </p>
 		</div>
 		<div class="pic">
 			<img src="https://picsum.photos/600/350?random=40" alt="">
 		</div>

 	</div>
</div>
</template>

<style lang="scss" scoped>
.wrap {
	width: 960px;
	margin: 0 auto;
}

.item {
	display: flex;
	align-items: center;
	margin-bottom: 70px;
	img {
		width: 100%;
		vertical-align: middle;
		box-shadow: 0 0 5px 3px rgba($color: #000000, $alpha: 0.3);
	}
	//flex 收縮值為0
	.pic,
	.text {
		flex-shrink: 0;
		width: 50%;
	}
	.text {
		padding: 20px 30px;
		//因為要讓文字在上，所以可使用相對定位，並讓其排序比其他元素較高
		position: relative;
		z-index: 2;
		border-radius: 6px;
		box-shadow: 0 0 5px 3px rgba($color: #000000, $alpha: 0.3);

		h2 {
			font-size: 32px;
			color: #167bff;
		}
		p {
			line-height: 2;
		}
	}
	//item 裡面第一層的第一個物件
	//子代選取器 http://csscoke.com/2013/10/14/was-framed-and-forgotten-ie6-css-selectors/
	> :first-child {
		margin-right: -40px;
	}

	//重要的部分
	&:nth-child(1) .text {
		background-color: rgba($color:#fdf5e6, $alpha: 0.5);

	}
	&:nth-child(2) .text {
		background-color: rgba($color:#fdf5e6, $alpha: 0.5);
	}
	&:nth-child(3) .text {
		background-color: rgba($color:#fdf5e6, $alpha: 0.5);
	}
	&:nth-child(4) .text {
		background-color: rgba($color:#fdf5e6, $alpha: 0.5);
	}
}

</style>