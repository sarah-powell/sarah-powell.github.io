<script>
    export let title = "Title"
    export let description = "Lorem ipsum dolor sit amet, consectetur adipiscing elit..."
    export let date = "Jan 1, 1970"
</script>


<div class="Tile">
    <div class="title">{title}</div>
    <div class="description">{description}</div>
    <div class="date">{date}</div>
</div>

<style>

    .Tile {
        background-color: #395E43;
        color: white;
        display: flex;
        margin: 8px;
        padding: 8px;
        border-radius: 10px;
        
        width: 120px;
        min-height: 70px;

        flex-direction: column;
        justify-content: space-between;
        row-gap: 8px;
    }
    
    .description {
        font-size: 12px;
    }

    .date {
        font-style: italic;
        font-size: 14px;
    }

</style>