<script type="ts">
	import '../app.css';
	import Footer from '../lib/components/footer.svelte';
	import Header from '../lib/components/header.svelte';
	import Container from '../lib/components/container.svelte';
</script>

<Header />
<Container>
	<slot />
</Container>
<Footer />
