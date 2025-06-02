<script>
    import { base } from '$app/paths';
</script>

<div class="fixed inset-0 -z-10 h-full w-full bg-white bg-[linear-gradient(to_right,#8080800a_1px,transparent_1px),linear-gradient(to_bottom,#8080800a_1px,transparent_1px)] bg-[size:14px_24px]"></div>

<div id="banner" class="bg-gradient-to-b from-stone-50 to-stone-50">
    <div class=directory>
        <button type="button">Home</button>
        <button type="button">Projects</button>
        <a href="{base}/blog">Blog</a>
    </div>
</div>

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

    <div class=block>

        <h2>Projects</h2>
        <div class = project>
            <img src="{base}/placeholder.jpg">
            <div class = block>
                <h3>project 1</h3>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nam arcu nisl, congue et quam sed, aliquam viverra nisi. Sed ornare at dolor non vehicula.</p>
            </div>
        </div>
        <div class = project>
            <img src="{base}/placeholder.jpg">
            <div class = block>
                <h3>project 1</h3>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nam arcu nisl, congue et quam sed, aliquam viverra nisi. Sed ornare at dolor non vehicula.</p>
            </div>
        </div>

    </div>

    <div class=block>
        <h2>Blog</h2>
        <div class = card-slider>
            <div class = card>
                <img src="{base}/placeholder.jpg">
                <div class="card-text">title</div>
                
            </div>
        </div>
    </div>

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

    .project{
        display:flex;
        gap: 10px;
        flex-wrap:wrap;
        
    }

    .project img{
        width: clamp(300px,30%, 200px);
    }

    .project .block{
        flex:1;
        min-width:150px;
    }

    .block{
        display:flex;
        flex-direction: column;
        gap: 30px;
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