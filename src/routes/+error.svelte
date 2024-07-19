<script>
	import { page } from '$app/stores';
</script>

<section>
    <h3>Oops. It looks like this page is not available.</h3>
    <p>{$page.error ? $page.error.message : ''}</p>
</section>
