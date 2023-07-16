<script>
    let name = 'world';
    let count = 0;
</script>

<p>Regular js {count}</p>
    <button on:click={() => count +=1}>
        Clicked {count} times</button>
