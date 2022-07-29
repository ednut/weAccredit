<script lang="ts">
	import { page } from '$app/stores';
</script>

<header class="flex justify-between items-center px-8 lg:px-12 pt-8 font-tt container mx-auto">
	<a href="/"><img class="w-48" src="/assets/images/svg/logo.svg" alt="logo" /></a>
	<ul class="m-0 p-0 hidden md:block font-semibold">
		<li class="inline-block mr-8" class:font-extrabold={$page.url.pathname === '/'}>
			<a href="/">About</a>
		</li>
		<li
			class="inline-block"
			class:font-extrabold={$page.url.pathname === '/accredited' ||
				$page.url.pathname === '/accredited/schedule' ||
				$page.url.pathname === '/accredited/payment'}
		>
			<a href="/accredited">Become accredited</a>
		</li>
	</ul>
	<ul class="m-0 p-0 md:hidden">
		<li><label for=""><img src="/assets/images/svg/icons-menu.svg" alt="" /></label></li>
	</ul>
</header>
