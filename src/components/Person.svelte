<script>
    export let name;
    export let lastName;
    export let age;
    export let someNullValue
</script>

<style>
    p {
        color: var(--theme-color);
        font-size: 22px;
    }
</style>

<div class="Person">
    <p>Name: {name} {lastName}. Age: {age} </p>
    {#if someNullValue}
        <p>{someNullValue}</p>
    {/if}
</div>
