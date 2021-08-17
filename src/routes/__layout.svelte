<script>
    import "../app.postcss";
    import Nav from "$lib/Nav.svelte";
    import Main from "$lib/Main.svelte";
</script>

<Nav title="Lending Hands"/>

<Main>
    <slot></slot>
</Main>