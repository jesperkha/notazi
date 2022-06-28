<script>
	let isLoggedIn = false
</script>

<section>
	<div class="content">
		<p id="logo">notazi</p>
		<p id="separator" />

		<ul>
			<li><a href="/">My notes</a></li>
			<li><a href="/">Some link</a></li>
		</ul>

		<!-- Todo: make login align to right border -->
		<div class="login">
			{#if isLoggedIn}
				<p>username</p>
				<!-- icon -->
			{:else}
				<a href="/">Log in</a>
			{/if}
		</div>
	</div>
</section>

<style>
	section {
		width: 100%;
		height: 5em;
		display: flex;
		justify-content: center;
		align-items: center;
		background-color: white;
		box-shadow: 0 0 1em 0em rgba(0, 0, 0, 0.05);
	}

	/* content box for links */
	.content {
		width: 50%;
		height: 100%;
		display: flex;
		align-items: center;
	}

	#logo {
		font-family: "Dosis";
		font-size: 2em;
		margin-bottom: 0.3em;
	}

	#separator {
		margin: 1em;
		margin-left: 2em;
		width: 2px;
		height: 40%;
		background-color: rgba(0, 0, 0, 0.1);
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
