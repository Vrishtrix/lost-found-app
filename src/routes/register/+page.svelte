<script>
	import { enhance } from '$app/forms';
</script>

<div class="grid grid-cols:2@sm min-h:100vh">
	<div
		class="bg:url('/images/login-bg.jpg') bg:center|no-repeat hidden block@sm"
	/>

	<div class="flex flex:col p:50 ai:center jc:space-between">
		<div class="flex ai:center gap:20">
			<img src="/images/logo.png" alt="logo" class="w:50" />
			Lost Found.
		</div>

		<div class="flex flex:col w:full ai:center gap:50">
			<h1>Register a new account.</h1>

			<form
				method="POST"
				class="flex flex:col gap:10 min-w:50% w:full w:auto@sm"
				use:enhance
			>
				<label for="username" class="fg:gray-30">
					Registration Number:
				</label>
				<input
					type="text"
					name="username"
					id="username"
					placeholder="98ABC01234"
					class="p:15 r:10 b:1|solid|gray-80"
					required
				/>
				<br />
				<label for="password" class="fg:gray-30"> Password: </label>
				<input
					type="password"
					name="password"
					id="password"
					placeholder="&#9679;&#9679;&#9679;&#9679;&#9679;&#9679;&#9679;&#9679;&#9679;&#9679;"
					class="p:15 r:10 b:1|solid|gray-80"
					required
				/>

				<input
					type="submit"
					value="Sign Up"
					class="my:15 py:15 bg:black fg:white r:10"
				/>
			</form>
		</div>

		<a href="/" class="f:14 fg:gray-60">
			Have an account already? Log in.
		</a>
	</div>
</div>
