<script>
	import { page } from '$app/stores';
</script>

<div class="space-10"></div>

<section>
    <h3>Oops. It looks like this page is not available.</h3>
    <blockquote>{$page.error ? $page.error.message : ''}</blockquote>
</section>

<div class="space-10"></div>
<div class="space-10"></div>