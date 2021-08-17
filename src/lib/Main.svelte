<script>
    import Container from "./Container.svelte";
    import Column from "./Column.svelte";
</script>

<main class="min-h-screen pb-8">
    <Container inset>
        <Column>
            <slot></slot>
        </Column>
    </Container>
</main>