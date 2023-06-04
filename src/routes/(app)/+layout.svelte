<script>
	//@ts-ignore
	import SvelteTooltip from 'svelte-tooltip';

	import { LayoutList, User } from 'lucide-svelte';
</script>

<div class="flex flex:col gap:40 px:5vw w:full min-h:100vh">
	<div
		class="grid grid-cols:2@sm pt:10 pb:5 gap:25 w:full bb:1|solid|gray-80"
	>
		<a
			href="/dashboard"
			class="flex gap:20 ai:center jc:center jc:flex-start@sm"
		>
			<img src="/images/logo.png" alt="logo" class="w:50" />
			Lost Found.
		</a>

		<div class="flex ai:center jc:center jc:flex-end@sm gap:50">
			<div class="flex ai:center gap:10">
				<button
					class="fg:white bg:gray-90:hover cursor:pointer p:10 r:10"
				>
					<SvelteTooltip tip="My Items" color="#000" bottom>
						<LayoutList color="#000" />
					</SvelteTooltip>
				</button>

				<a
					href="/profile"
					class="fg:white bg:gray-90:hover cursor:pointer p:10 r:10"
				>
					<SvelteTooltip tip="Profile" color="#000" bottom>
						<User color="#000" />
					</SvelteTooltip>
				</a>
			</div>

			<button class="my:15 py:15 px:25 bg:black fg:white r:10">
				List a new request
			</button>
		</div>
	</div>

	<slot />
</div>
