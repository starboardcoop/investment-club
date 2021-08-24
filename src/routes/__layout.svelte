<script>
    import "../app.postcss";
    import Nav from "$lib/Nav.svelte";
    import Main from "$lib/Main.svelte";
    import Footer from "$lib/Footer.svelte";
    import Row from "$lib/Row.svelte";
    import Button from "$lib/Button.svelte";
    import MoneySvg from "$lib/MoneySvg.svelte";
</script>

<div class="z-0 fixed w-4/6 text-gray-800 bottom-2 right-8 lg:top-32 lg:left-16">
    <MoneySvg />
</div>

<div class="flex flex-col min-h-screen">
    <Nav title="Lending Hands"/>
    <Main>
        <slot></slot>
    </Main>
    <Footer>
        <Row>
            <Button type="ghost"><a href="https://starboard.coop/" target="_blank">Built by Starboard</a></Button>
        </Row>
    </Footer>
</div>