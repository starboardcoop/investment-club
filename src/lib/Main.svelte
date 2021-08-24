<script>
    import Container from "./Container.svelte";
    import Column from "./Column.svelte";
</script>

<main class="flex-grow pb-8">
    <Container inset>
        <Column>
            <slot></slot>
        </Column>
    </Container>
</main>