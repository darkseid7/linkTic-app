<script lang="ts">
	export let label: string = '';
	export let width: string = '';
	export let type: string = 'primary';
</script>

{#if type === 'primary'}
	<button class="{width ? width : 'w-full'} rounded-lg text-white py-4 bg-primary-800">
		{label}
	</button>
{:else if type === 'secondary'}
	<button
		class="{width ? width : 'w-full'} 
            rounded-lg text-primary-800 py-4 bg-white border border-primary-800"
	>
		{label}
	</button>
{:else if type === 'danger'}
	<button class="{width ? width : 'w-full'} rounded-lg text-white py-4 bg-error-400">
		{label}
	</button>
{/if}
