<script lang="ts">
	import { cn } from '$lib/utils/cn';

	let className: string | undefined = undefined;

	export { className as class };
	export let backgroundImage =
		'https://images.unsplash.com/photo-1631947430066-48c30d57b943?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1432&q=80';
</script>

<div
	class={cn('absolute inset-0 bg-cover', className)}
	style="background-image: url({backgroundImage});"
/>

<!-- bottom black/80 to transaprent top-->
<div class="absolute inset-0 bg-gradient-to-t from-black to-transparent" />

<slot />
