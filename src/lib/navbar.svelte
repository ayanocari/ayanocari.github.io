<script>
  import { base } from '$app/paths';
</script>

  
<div id="banner">
  <img id="book" src="{base}/top-notebook.png">
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
    position:absolute;
    display:flex;
    gap: min(5vw, 60px);
  }


  #book {
    width: clamp(700px, 70vw, 1500px);
    transform:translateY(max(-20vw, -400px));
  }
  
  
</style>