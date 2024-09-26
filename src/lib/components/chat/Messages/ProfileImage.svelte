<script lang="ts">
	import { settings } from '$lib/stores';
	import ProfileImageBase from './ProfileImageBase.svelte';

	export let className = 'max-w-[80px]';
	export let src = '';
</script>

<div class={`flex-shrink-0 ${($settings?.chatDirection ?? 'LTR') === 'LTR' ? 'mr-3' : 'ml-3'}`}>
	<ProfileImageBase {src} {className} />
</div>
