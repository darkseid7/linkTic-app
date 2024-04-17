<script lang="ts">
	import { Icon } from '$lib';
	import { page, navigating } from '$app/stores';

	let menuOptions = [
		{
			name: 'Home',
			icon: 'Home',
			link: '/'
		},
		{
			name: 'Products',
			icon: 'Box',
			link: '/products'
		},
		{
			name: 'Orders',
			icon: 'Clipboard',
			link: '/orders'
		}
	];
</script>

<div class="py-10 px-6 h-screen">
	<div class="flex justify-center py-10">
		<h1>LOGO</h1>
	</div>

	<nav>
		<ul class="flex flex-col">
			{#each menuOptions as option}
				<li
					class="rounded-lg {$page.url.pathname === option.link
						? 'bg-primary-600 text-white'
						: 'hover:bg-gray-200'}"
				>
					<a class="py-3.5 px-4 flex items-center gap-3" href={option.link}>
						<Icon name={option.icon} fill={$page.url.pathname === option.link ? '#fff' : '#000'} />
						{option.name}
					</a>
				</li>
			{/each}
		</ul>
	</nav>
</div>
