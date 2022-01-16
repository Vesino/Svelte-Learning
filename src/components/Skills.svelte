<script>
    let skills = [
        {
            id: 1,
            name: 'Play Giuitar'
        },
        {
            id: 2,
            name: 'Python'
        },
        {
            id: 3,
            name: 'JavaScript'
        }
    ]
</script>

<style>
    ul {
        display: flex;
        align-items: flex-start;
        flex-direction: column;
        margin: 0;
        padding: 0;
        list-style: none;
    }
    li {
        margin-bottom: 5px;
    }
</style>

<div class="Skills">
    <h3>Habilidades</h3>
    <ul>
        {#each skills as {name}, i}
        <li>{name}</li>
        {/each}
    </ul>
</div>