<script>
	import '../app.css';
	import { base } from '$app/paths';
	
	let { children } = $props();
</script>
<!-- 
<div id="banner">
	<div class=directory>
        <button type="button">Home</button>
        <button type="button">Projects</button>
        <a href="{base}/blog">Blog</a>
    </div>
</div>

<style>
	#banner{
        height:5vh;
        width:100vw;
        position:fixed;

        display:flex;
        align-items:center;
        justify-content:center;

        border-bottom:2px rgb(195, 194, 236) solid;
    }

    .directory{
        display:flex;
        gap: min(5vw, 60px);
    }
</style> --> 

{@render children()}