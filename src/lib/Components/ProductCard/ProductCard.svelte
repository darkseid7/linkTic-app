<script lang="ts">
	interface Product {
		link: string;
		image: string;
		name: string;
		description: string;
		reference: string;
		price: number;
	}

	export let product: Product;
</script>

<div class="w-full bg-gray-50 rounded-lg overflow-hidden hover:bg-gray-100">
	<a href={product.link}>
		<div class="w-full bg-cover bg-no-repeat overflow-hidden">
			<img
				class="w-full h-full object-cover object-center"
				src={product.image}
				alt={product.name}
			/>
		</div>
		<div class="w-full flex flex-col p-6">
			<h3 class="text-xl font-bold mb-2">{product.name}</h3>
			<p>{product.description}</p>
			<p>Reference: <strong>{product.reference}</strong></p>
			<p>Price: <strong>${product.price}</strong></p>
		</div>
	</a>
</div>
