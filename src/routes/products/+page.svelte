<script>
	import { ProductCard } from '$lib';

	let productsArray = [
		{
			name: 'Product 1',
			image: 'https://picsum.photos/200',
			description: 'This is a description of Product 1',
			reference: '123456',
			price: 100,
			link: '/products/1'
		},
		{
			name: 'Product 2',
			image: 'https://picsum.photos/200',
			description: 'This is a description of Product 2',
			reference: '123457',
			price: 200,
			link: '/products/2'
		},
		{
			name: 'Product 3',
			image: 'https://picsum.photos/200',
			description: 'This is a description of Product 3',
			reference: '123458',
			price: 300,
			link: '/products/3'
		},
		{
			name: 'Product 4',
			image: 'https://picsum.photos/200',
			description: 'This is a description of Product 4',
			reference: '123459',
			price: 400,
			link: '/products/4'
		},
		{
			name: 'Product 5',
			image: 'https://picsum.photos/200',
			description: 'This is a description of Product 5',
			reference: '123460',
			price: 500,
			link: '/products/5'
		},
		{
			name: 'Product 6',
			image: 'https://picsum.photos/200',
			description: 'This is a description of Product 6',
			reference: '123461',
			price: 600,
			link: '/products/6'
		},
		{
			name: 'Product 7',
			image: 'https://picsum.photos/200',
			description: 'This is a description of Product 7',
			reference: '123462',
			price: 700,
			link: '/products/7'
		},
		{
			name: 'Product 8',
			image: 'https://picsum.photos/200',
			description: 'This is a description of Product 8',
			reference: '123463',
			price: 800,
			link: '/products/8'
		},
		{
			name: 'Product 9',
			image: 'https://picsum.photos/200',
			description: 'This is a description of Product 9',
			reference: '123464',
			price: 900,
			link: '/products/9'
		},
		{
			name: 'Product 10',
			image: 'https://picsum.photos/200',
			description: 'This is a description of Product 10',
			reference: '123465',
			price: 1000,
			link: '/products/10'
		},

		{
			name: 'Product 11',
			image: 'https://picsum.photos/200',
			description: 'This is a description of Product 11',
			reference: '123466',
			price: 1100,
			link: '/products/11'
		},
		{
			name: 'Product 12',
			image: 'https://picsum.photos/200',
			description: 'This is a description of Product 12',
			reference: '123467',
			price: 1200,
			link: '/products/12'
		},
		{
			name: 'Product 13',
			image: 'https://picsum.photos/200',
			description: 'This is a description of Product 13',
			reference: '123468',
			price: 1300,
			link: '/products/13'
		},
		{
			name: 'Product 14',
			image: 'https://picsum.photos/200',
			description: 'This is a description of Product 14',
			reference: '123469',
			price: 1400,
			link: '/products/14'
		},
		{
			name: 'Product 15',
			image: 'https://picsum.photos/200',
			description: 'This is a description of Product 15',
			reference: '123470',
			price: 1500,
			link: '/products/15'
		},
		{
			name: 'Product 16',
			image: 'https://picsum.photos/200',
			description: 'This is a description of Product 16',
			reference: '123471',
			price: 1600,
			link: '/products/16'
		},
		{
			name: 'Product 17',
			image: 'https://picsum.photos/200',
			description: 'This is a description of Product 17',
			reference: '123472',
			price: 1700,
			link: '/products/17'
		},
		{
			name: 'Product 18',
			image: 'https://picsum.photos/200',
			description: 'This is a description of Product 18',
			reference: '123473',
			price: 1800,
			link: '/products/18'
		}
	];
</script>

<section class="my-12 mx-9">
	<div class="flex flex-col gap-12">
		<h2 class="text-5xl font-bold text-center">Product Catalog</h2>

		<div class="grid grid-cols-3 gap-4">
			{#each productsArray as product}
				<ProductCard {product} />
			{/each}
		</div>
	</div>
</section>
