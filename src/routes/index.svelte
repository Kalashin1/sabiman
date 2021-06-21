<script>
	import Jumbotron from '../components/Jumbotron.svelte'
	import Carousel from '../components/Carousel.svelte'
	import WorkingMode from '../components/Work.svelte'
	import Services from '../components/Services.svelte'
	import PageContent from '../components/PageContent.svelte'
</script>


<svelte:head>
	<title>Sabiman - Home</title>
</svelte:head>

<section>
	<Carousel />
	<Jumbotron />
	<WorkingMode />
	<Services />
	<PageContent />
</section>

