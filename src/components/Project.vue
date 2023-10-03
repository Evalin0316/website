<template>
	<div>
		<div class="item">
			<div class="pic">
				<img src="../assets/image/sign.png" alt="">
			</div>
			<div class="text">
				<h2>點點簽(F2E 4TH活動競賽題目)</h2>
				<ul>
					<li>點點簽是一個線上文件簽署平台，提供使用者可以即時上傳文件預覽以及建立簽名並進行簽署與下載。</li>
					<li>與後端討論API資料串接格式</li>
				</ul>
				<div>
					<TagItem :TagItem="['Vue3','Canvas','PDF.js','fabric.js','jsPDF']"/>
				</div>
			</div>
		</div>

		<!-- item02 -->
		<div class="item">
			<div class="text">
				<h2>F2E活動網站(F2E 4TH活動團體競賽)</h2>
				<ul>
					<li>使用GSAP實作滾動式視差與動畫</li>
					<li>與UIUX設計師討論layout規劃</li>
				</ul>
				<div>
					<TagItem :TagItem="['Vue3','GSAP']"/>
				</div>
				<div>LINK</div>
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
				<h2>服飾電商平台</h2>
				<ul>
					<li>製作使用者購物前台以及管理者後台</li>
					<li>使用Axois串接API</li>
				</ul>
				<div>
					<TagItem :TagItem="['Vue3']"/>
				</div>
				<div>LINK</div>
			</div>
		</div>

		<!-- item04 -->
		<div class="item">
			<div class="text">
				<h2>代辦事項</h2>
				<p>使用React開發簡易版的代辦事項網站。包含串接使用者登入登出，新增刪除等功能。</p>
				<div>
					<TagItem :TagItem="['React','react-hook-form']"/>
				</div>
				<div>LINK</div>
			</div>
			<div class="pic">
				<img src="https://picsum.photos/600/350?random=40" alt="">
			</div>
		</div>
	</div>
</template>

<script>
import TagItem from '../layout/Tag';
export default{
	components: {
        TagItem
	},
	setup() {
		
	},
}
</script>


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

	.pic,
	.text {
		flex-shrink: 0;
		width: 50%;
	}

	.text {
		padding: 20px 30px;
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

	> :first-child {
		margin-right: -40px;
	}

	&:nth-child(1) .text {
		background-color: rgba($color: #fdf5e6, $alpha: 0.5);

	}

	&:nth-child(2) .text {
		background-color: rgba($color: #fdf5e6, $alpha: 0.5);
	}

	&:nth-child(3) .text {
		background-color: rgba($color: #fdf5e6, $alpha: 0.5);
	}

	&:nth-child(4) .text {
		background-color: rgba($color: #fdf5e6, $alpha: 0.5);
	}
}
</style>