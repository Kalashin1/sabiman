<script>
	import Header from "../components/Header.svelte"
	import Footer from "../components/Footer.svelte"
	
	export let segment;
</script>




<main id="wrapper">
	<Header {segment} />
	<main id="core">
		<slot></slot>
	</main>
	<Footer {segment} />
</main>