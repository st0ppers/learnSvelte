<script>
    import ContentCard from "./ContentCard.svelte";
    import IfStatements from "./IfStatements.svelte";

    let name = 'world';
    let count = 0;
    let title = 'My title';
    let jobTitle = 'Software Engineer';
    let isDone = false;

    let userName = 'world';
    let discription = 'Software Engineer';
    $: uppercaseName = name.toUpperCase();

    $: {
        console.log(`Hello ${name}!`);
    }

    function handleInput(event) {
        name = event.target.value;
    }

</script>

<p>Regular js {count}</p>
<p>Uppercase name {uppercaseName}</p>

<button on:click={() => count +=1}>Clicked {count} times</button>

<input bind:value={name} type="text"/>
<input bind:value={title} type="text"/>
<input bind:value={jobTitle} type="text"/>
<!--<input on:input={handleInput} type="text">-->

<IfStatements bind:isDone/>
<ContentCard {title} {discription} {userName}/>
