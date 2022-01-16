<script>
    let count = 0

    const handleClick = (event) => {
        count += 1
    }

</script>


<button on:click={handleClick}>Click {count === 0 ? '' : count}</button>
