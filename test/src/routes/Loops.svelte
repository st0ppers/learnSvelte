<script>
    export let nums;
    let s = 0;
</script>

{#each nums as num}
    {s += 0 + num}
{/each}
<p>{s}</p>