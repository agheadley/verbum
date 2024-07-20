<script>
	import { page } from '$app/stores';
</script>

<p>&nbsp;</p>
<p>&nbsp;</p>

<section>
    <h3>Oops. It looks like this page is not available.</h3>
    <blockquote>{$page.error ? $page.error.message : ''}</blockquote>
</section>

