<script lang="ts">
	let { data } = $props();

	const logout = async () => {
		await data.supabase.auth.signOut();
	};
</script>

<h1>Welcome to Supabase!</h1>
{#if data.session}
	<p>You are logged as {data.session.user.email}</p>
	<button onclick={logout}>logout </button>
{:else}
	<p>You are not logged in</p>
	<a href="/auth">login</a>
{/if}
