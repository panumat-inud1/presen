<script lang="ts">
	import image1 from '$lib/images/1.png';
	import image2 from '$lib/images/2.png';
	import image3 from '$lib/images/3.png';
	import image4 from '$lib/images/4.png';
	import image5 from '$lib/images/5.png';
	import image6 from '$lib/images/6.png';
	import image7 from '$lib/images/sytem.png';

	let images = [
		{ scr: image1, decription: 'GAME CARD' },
		{ scr: image2, decription: '' },
		{ scr: image3, decription: '' },
		{ scr: image4, decription: '' },
		{ scr: image5, decription: '' },
		{ scr: image6, decription: '' },
		{ scr: image7, decription: 'System Hospital' }
	];
</script>

<h3>FONTEND(ไม่ยืดติดแล้วแต่งาน)</h3>
<p>-Svelte</p>
<p>-Sveltekit</p>
<p>-node.js</p>

<h3>BACKEND(ไม่ยืดติดแล้วแต่งาน)</h3>
<p>-python</p>
<p>-Fastapi</p>
<p>-Tortoise ORM</p>

<h3>DATABASE(ไม่ยืดติดแล้วแต่งาน)</h3>
<p>-Postgresql</p>
<p>-oracle</p>

<h4>RESPONSIVE</h4>
<p>Ios Android</p>

<h5>Skill Play</h5>
<p>vue.js , asp.net , php , vb.net , mysql , sqlserver</p>

<lu>
        <li>ตัวอย่างคราวๆ</li>
	{#each images as { scr, decription }, i}
		<li>{decription}</li>
		<li><img class="imag" src={scr} alt="" srcset="" /></li>
	{/each}
</lu>

<style lang="css">
	.imag {
		object-fit: contain;
		width: 320px;
	}
	li {
		list-style: none;
		display: flex;
		justify-content: center;
		padding-top: 10px;
	}

	@media (min-width: 768px) {
		.imag {
		
		width: auto;
	}
	}
</style>
