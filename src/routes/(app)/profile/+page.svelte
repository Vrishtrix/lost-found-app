<script lang="ts">
	import { enhance } from '$app/forms';
	import { FileInput } from 'lucide-svelte';

	let avatarUpload: any;
</script>

<div
	class="bg:url('/images/login-bg.jpg') bg:center|no-repeat flex flex:col ai:center w:full p:50 r:10"
>
	<div class="flex ai:center gap:50 bg:white r:10 p:25">
		<img
			src="/images/avatar.jpg"
			alt="Profile Avatar"
			width={100}
			class="round"
		/>
		<div class="flex flex:col gap:15">
			<h1>Vrishin Patel</h1>
			<p class="fg:gray-60">21BCE0275</p>
		</div>
	</div>
</div>

<div class="flex jc:space-between ai:center f:bold">
	<span>Edit Profile</span>
	<button class="bg:red fg:white px:20 py:15 r:10"> Log Out </button>
</div>

<div>
	<form
		use:enhance
		class="flex jc:space-between flex:wrap gap:20 ai:center w:full"
	>
		<label for="fname" class="fg:gray-30"> First Name: </label>
		<input
			type="text"
			name="fname"
			id="fname"
			placeholder="Vrishin"
			class="p:15 r:10 b:1|solid|gray-80"
			required
		/>

		<label for="lname" class="fg:gray-30"> Last Name: </label>
		<input
			type="text"
			name="lname"
			id="lname"
			placeholder="Patel"
			class="p:15 r:10 b:1|solid|gray-80"
			required
		/>

		<label for="email" class="fg:gray-30"> E-mail: </label>
		<input
			type="email"
			name="email"
			id="email"
			placeholder="vrishin.u@gmail.com"
			class="p:15 r:10 b:1|solid|gray-80"
			required
		/>

		<label for="phone" class="fg:gray-30"> Phone: </label>
		<input
			type="tel"
			name="phone"
			id="phone"
			placeholder="+916361411494"
			class="p:15 r:10 b:1|solid|gray-80"
			required
		/>

		<button type="submit" class="my:15 py:15 px:10 bg:black fg:white r:10">
			Save Changes
		</button>
	</form>
</div>

<span class="f:bold"> Edit Avatar </span>

<!-- svelte-ignore a11y-click-events-have-key-events -->
<div
	class="flex flex:col ai:center jc:center gap:20 b:1|dashed|gray-80 p:25 r:10"
	on:click={() => {
		avatarUpload.click();
	}}
>
	<FileInput />
	Choose image
</div>

<input
	class="hidden"
	type="file"
	accept=".jpg, .jpeg, .png"
	bind:this={avatarUpload}
/>
