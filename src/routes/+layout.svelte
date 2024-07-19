<script>
	import '../simple.css';
	import { page } from '$app/stores'; 
	
	import {UserIcon,SettingsIcon} from 'svelte-feather-icons';

	let menu={
		links:[
			{txt:'Overview',path:'/'},
			{txt:'Edit',path:'/edit'},
			{txt:'Preferences',path:'/preferences'},

		]
	};
</script>

<div class="app">
	<header>
		<nav>
			<a href='/' class={$page.url.pathname==='/' ? 'current' : ''}>Home</a>
			<a href='/settings' class={$page.url.pathname==='/settings' ? 'current' : ''}><SettingsIcon size="16"/></a>
				
		</nav>
		<h3>Verbum</h3>
		<p>A svelte5 test app</p>
	
		
	</header>
	<main>
		<slot />
	</main>

	<footer>
		<p>visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to learn SvelteKit</p>
	</footer>
</div>

<style>

</style>
