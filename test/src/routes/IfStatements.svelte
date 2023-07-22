<script>
    import ContentCard from "./ContentCard.svelte";
    import Loops from "./Loops.svelte";

    export let isDone;

    let userName = 'world';
    let title = 'My title';
    let discription = 'Software Engineer';
    const check = () => {
        isDone = !isDone;
    }
</script>

<button on:click={check}>Is done = true</button>
{#if isDone}
    <Loops nums={[0,1,2,3,4]}/>
    <ContentCard
            {userName}
            {title}
            {discription}
    />
{/if}