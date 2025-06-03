<script>
    import { base } from '$app/paths'
    import Card from '$lib/description-card.svelte'
    import Block from '$lib/text-block.svelte'
    import Navbar from '$lib/navbar.svelte'
</script>

<Navbar isHomepage={false} />

<div id="main-content">

    <Block>
        <Card title="Hello" description="testing" img="{base}/placeholder.jpg"></Card>
    </Block>  

    <Block>
        <Card title="Hello" description="testing" img="{base}/placeholder.jpg"></Card>
    </Block>  

</div>