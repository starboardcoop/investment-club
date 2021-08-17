<script>
    import "../app.postcss";
    import Nav from "$lib/Nav.svelte";
    import Main from "$lib/Main.svelte";
    import Footer from "$lib/Footer.svelte";
    import Row from "$lib/Row.svelte";
    import Button from "$lib/Button.svelte";
</script>

<Nav title="Lending Hands"/>
<Main>
    <slot></slot>
</Main>
<Footer>
    <Row>
        <Button type="ghost"><a href="https://starboard.coop/" target="_blank">Built by Starboard</a></Button>
    </Row>
</Footer>