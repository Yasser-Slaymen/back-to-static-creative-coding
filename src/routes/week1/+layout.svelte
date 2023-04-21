<script>
  import Header from "$lib/components/Header.svelte";
  import Footer from "$lib/components/Footer.svelte";
  import "../styles.css";
</script>
<div class="app">
 <Header />
 <main>
	<slot/>
 </main>
 <Footer />
</div>
<style>
	.app {
		display: flex;
		flex-direction: column;
		justify-content: center;
		min-height: 50vh;
		max-width: 100vw;
		overflow: hidden;
	}

	main {
		flex: 1;
		display: flex;
		flex-direction: column;
		align-items: center;
		padding: 1rem;
		width: 100%;
		max-width: 64rem;
		margin: 0 auto;
		box-sizing: border-box;
	}
</style>