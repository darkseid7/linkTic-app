<script lang="ts">
	import * as icon from './Icons/index';

	export let name: string = 'Home';
	export let fill: string = '#000';
</script>

<svelte:component this={icon[name]} {fill} />
