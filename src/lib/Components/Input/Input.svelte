<script lang="ts">
	export let label: string = '';
	export let placeholder: string = '12345...';
	export let value: string = '';
	export let type: string = 'text';
</script>

<div class="w-full">
	<label class="label pb-1 pl-0">
		<span class="text-xs text-gray-600">{label}</span>
	</label>
	<input
		class="w-full pr-11 py-3 px-4 bg-gray-50 text-gray-900 rounded-lg placeholder:text-gray-600 hover:border-gray-400 focus:border-primary-800 focus:outline-none"
		{placeholder}
		{value}
		{type}
	/>
</div>
