<template>
	<div class="container m-auto">
		<div class="item flex justify-center flex-wrap flex-col md:flex-row">
			<div class="pic w-full md:w-1/2">
				<img class="" src="../assets/image/sign.png" alt="">
			</div>
			<div class="text bg-orange-50 w-full mt-3 md:w-1/2 md:mt-0">
				<div class="text-2xl font-bold mb-3 text-black">點點簽</div>
				<ul class="text-left list-disc px-8 text-black">
					<li>點點簽是一個線上文件簽署平台，提供使用者可以即時上傳文件預覽以及建立簽名並進行簽署與下載。</li>
					<li>與後端討論API資料串接格式</li>
					<li>使用Vue Router 完成路由管理</li>
					<li>使用Tailwind CSS實現畫面 </li>
				</ul>
				<div class="mt-4">
					<TagItem :TagItem="['Vue3','Canvas','PDF.js','fabric.js','jsPDF']"/>
				</div>
				<a href="https://evalin0316.github.io/SIGN/" target="_blank">
					<button class="text-white hover:text-white mt-4 ml-2.5 px-10 py-3 bg-black  rounded cursor-pointer hover:bg-slate-500">
						LINK
					</button>
				</a>
			</div>
		</div>

		<div class="item flex justify-center flex-wrap flex-col md:flex-row">
			<div class="text bg-orange-50 w-full mt-3 md:w-1/2 md:mt-0">
				<div class="text-2xl font-bold mb-3 text-black">F2E活動網站(F2E 4TH活動團體競賽)</div>
				<ul class="text-left list-disc px-8 text-black">
					<li>使用GSAP實作滾動式視差與動畫</li>
					<li>與UIUX設計師討論layout規劃</li>
				</ul>
				<div class="mt-4">
					<TagItem :TagItem="['Vue3','GSAP']"/>
				</div>
				<a href="https://f2e4th.github.io/week1/dist/" target="_blank">
					<button class="text-white hover:text-white mt-4 ml-2.5 px-10 py-3 bg-black  rounded cursor-pointer hover:bg-slate-500">
						LINK
					</button>
				</a>
			</div>
			<div class="pic w-full md:w-1/2">
				<img src="../assets/image/f2e-page.png" alt="">
			</div>
		</div>

		<div class="item flex justify-center flex-wrap flex-col md:flex-row">
			<div class="pic w-full md:w-1/2">
				<img src="../assets/image/nature.png" alt="">
			</div>
			<div class="text bg-orange-50 w-full mt-3 md:w-1/2 md:mt-0">
				<div class="text-2xl font-bold mb-3 text-black">服飾電商平台</div>
				<ul class="text-left list-disc px-8 text-black">
					<li>使用Vue.js開發一個現代化的電子商務平台</li>
					<li>實現商品目錄、購物車、結帳流程等核心功能。</li>
					<li>使用Vue Router 完成路由管理</li>
				</ul>
				<div class="mt-4">
					<TagItem :TagItem="['Vue3']"/>
				</div>
				<a href="https://evalin0316.github.io/Nature_store_shopping_cart/" target="_blank">
					<button class="text-white hover:text-white mt-4 ml-2.5 px-10 py-3 bg-black  rounded cursor-pointer hover:bg-slate-500">
						LINK
					</button>
				</a>
			</div>
		</div>

		<div class="item flex justify-center flex-wrap flex-col md:flex-row">
			<div class="text bg-orange-50 w-full mt-3 md:w-1/2 md:mt-0">
				<div class="text-2xl font-bold mb-3 text-black">代辦事項</div>
				<ul class="text-left list-disc px-8 text-black">
					<li>使用React.js開發簡易版的代辦事項網站。包含串接使用者登入登出，新增刪除等功能。</li>
				</ul>
				<div class="mt-4">
					<TagItem :TagItem="['React','react-hook-form']"/>
				</div>
				<a href="https://evalin0316.github.io/React-todoList/" target="_blank">
					<button class="text-white hover:text-white mt-4 ml-2.5 px-10 py-3 bg-black  rounded cursor-pointer hover:bg-slate-500">
						LINK
					</button>
				</a>
			</div>
			<div class="pic w-full md:w-1/2">
				<img src="../assets/image/todolist.png" alt="">
			</div>
		</div>
	</div>
</template>

<script>
import TagItem from '../layout/Tag.vue';
export default{
	components: {
        TagItem
	},
	setup() {
		
	},
}
</script>


<style lang="scss" scoped>
.container{
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
		// width: 50%;
	}

	.text {
		padding: 20px 30px;
		position: relative;
		z-index: 2;
		border-radius: 6px;
		box-shadow: 0 0 5px 3px rgba($color: #fdf5e6, $alpha: 0.3);

		p {
			line-height: 2;
		}
	}

	> :first-child {
		margin-right: 0;
		@media screen and (min-width:768px) {
			margin-right: -40px;
		}
	}
}

}

</style>