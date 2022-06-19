<script>
	let isLoggedIn = false
</script>

<section>
	<div>
		<p id="logo">notazi</p>
		<p id="separator" />

		<ul>
			<li><a href="/">My notes</a></li>
			<li><a href="/">Some link</a></li>
		</ul>

		{#if isLoggedIn}
			<p>username</p>
			<!-- icon -->
		{:else}
			<ul>
				<li><a href="/">Log in</a></li>
			</ul>
		{/if}
	</div>
</section>

<style>
	section {
		width: 100%;
		height: 5em;
		display: flex;
		justify-content: center;
		align-items: center;
	}

	div {
		width: 50%;
		height: 100%;
		display: flex;
		align-items: center;
		border-bottom: 1px solid black;
	}

	div:last-child {
		align-self: flex-end;
	}

	#logo {
		font-family: "Dosis";
		font-size: 2em;
		margin-bottom: 0.3em;
	}

	#separator {
		margin: 1em;
	}

	ul {
		display: flex;
		flex-direction: row;
	}

	li {
		list-style: none;
		margin: 1em;
		font-weight: 500;
		font-size: 0.8em;
	}

	a {
		padding: 1em;
		text-decoration: none;
		color: black;
	}
</style>
