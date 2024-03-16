<script>
    import Container from "./Container.svelte";
</script>

<Container>
    <div data-testid="text-input" contenteditable />

    <button data-testid="lock-button"> </button>

    <button data-testid="wonkier-button"> </button>

    <!--
        <p>FizzBuzz!</p> 

        should be rendered when the text inside the wonkier-button starts with FizzBuzz
    -->
</Container>
