<script lang="ts">
    import Block from '$lib/text-block.svelte';

    export let title: string;
    export let description: string;
    export let img: string;
</script>

<div class="description-card">
    <img src="{img}">
    <div class="block-wrapper">
        <Block>
            <h3>{title}</h3>
            <p>{description}</p>
        </Block>
    </div>
</div>

<style>
    .description-card{
            display:flex;
            gap: 10px;
            flex-wrap:wrap;
            
        }

    .description-card img{
            width: clamp(300px,30%, 200px);
        }

    .description-card .block-wrapper{
            flex:1;
            min-width:150px;
        }
</style>
 