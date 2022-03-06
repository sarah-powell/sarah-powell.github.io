<script>
    import { each } from "svelte/internal";
    import PostTile from "/src/PostTile.svelte";

    import "../app.css";

    let tiles = [
        {
            "title": "First post",
            "description": "Lorem ipsum dolor sit amet, consectetur...",
            "date": "Mar 6, 2022"
        },
        {
            "title": "Second post",
            "description": "Lorem ipsum dolor sit ",
            "date": "Jan 18, 2038"
        }
    ]
</script>

<svelte:head>
    <title>Sarah's Blog</title>
</svelte:head>

<div class="content">
    {#each tiles as tile}
        <PostTile {...tile}/>
        <PostTile {...tile}/>
        <PostTile {...tile}/>
        <PostTile {...tile}/>
        <PostTile {...tile}/>
        <PostTile {...tile}/>
        <PostTile {...tile}/>
        <PostTile {...tile}/>
        <PostTile {...tile}/>
        <PostTile {...tile}/>
    {/each}
</div>

<style>
    
    .content {
        display: flex;
        flex-direction: row;
        flex-wrap: wrap;
        flex-grow: 1;
        justify-content: center;

        margin: 20px 16px;
    }

    @media only screen and (min-width: 500px) {
        .content {
            margin: 20px 64px;
        }
    }
     
    @media only screen and (min-width: 800px) {
        .content {
            margin: 20px 256px;
        }
    }
</style>