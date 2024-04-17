<script>
	import '../app.css';

	import { SideMenu } from '$lib';
</script>

<main>
	<div class="flex">
		<div class="w-1/5 bg-gray-50 h-screen fixed">
			<SideMenu />
		</div>
		<div class="w-4/5 ml-auto">
			<slot></slot>
		</div>
	</div>
</main>
