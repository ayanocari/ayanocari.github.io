<script lang='ts'>
    import { base } from '$app/paths';
    import Card from '$lib/description-card.svelte'
    import Block from '$lib/text-block.svelte'
    import Navbar from '$lib/navbar.svelte'
</script>

<Navbar isHomepage={true} />

<div class="fixed inset-0 -z-10 h-full w-full bg-white bg-[linear-gradient(to_right,#8080800a_1px,transparent_1px),linear-gradient(to_bottom,#8080800a_1px,transparent_1px)] bg-[size:14px_24px]"></div>


<div id="color-block" class="bg-gradient-to-b from-indigo-300 from-0% via-cyan-200 via-70% to-white-0 to-90%">
    
    <div class=intro>
        
        <h1>I'm <br>Aya Nocari</h1>
        <p>Computer Science Student</p><br>

        <div class="social">
            
            <a href="https://www.linkedin.com/in/ayanocari/" target="blank">
                <img src="{base}/linkedin.svg" alt="Linkedin Icon via Bootstrap" width="32" height="32">
            </a>

            <a href="https://github.com/ayanocari" target="blank">
                <img src="{base}/github.svg" alt="Github Icon via Bootstrap" width="32" height="32">
            </a>

            <a href="mailto:nocariaya@gmail.com" target="blank">
                <img src="{base}/envelope.svg" alt="Envelope Icon via Bootstrap" width="32" height="32">
            </a>

        </div>

    </div>

</div>

<div id="main-content">

    <Block>
        <Card title="Hello" description="testing" img="{base}/placeholder.jpg"></Card>
    </Block>  

    <Block>
        <Card title="Hello" description="testing" img="{base}/placeholder.jpg"></Card>
    </Block>  

</div>

<style>

    .card{
        position:relative;
        display:inline-block;
    }

    .card img{
        display:block;
        width:100%;
        height: auto;
    }
    .card-text{
        position: absolute;
        top:0%;
        padding:10%;
        text-align: center;
    }

    #main-content{
        margin-right:20vw;
        margin-left:20vw;
        display:flex;
        flex-direction:column;
        gap: 15vh;
    }

    :root{
        --intro-height: 110vh;
    }

    #color-block{
        height:var(--intro-height);
    }

    .intro{
        height: calc(var(--intro-height)/1.2);
        
        display:flex;
        flex-direction: column;
        align-items:center;
        justify-content:center;

        text-align: center;
    }

    .intro h1{
        font-size:60px;
    }

    .social{
        display:flex;
        gap: 10px;

        margin-top: 5px;
    }


    


</style>