<style>
    .test {
        color: red;
    }
</style>

<script>
    export let userName;
    export let title;
    export let discription;
</script>

<div>
    <header>
        <div>
            <img src="" alt="">
        </div>
        <div>
            <h1 class:test={userName === 'test'}
            >{userName}</h1>
            <h2>{title}</h2>
        </div>
    </header>

    <div>
        <p>{discription}</p>
    </div>
</div>