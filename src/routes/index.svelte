<script>
    import Column from '$lib/Column.svelte';
    import Grid from '$lib/Grid.svelte';
    import Calculator from '$lib/Calculator.svelte';
</script>

<Column>
    <h1 class="w-4/5">We're a co-op that invests in co-ops.</h1>
    <Grid>
        <Column>
            <p>With a monthly investment to a local co-operative, you can grow your money while supporting sustainable business.</p>
        </Column>
        <Calculator />
    </Grid>
</Column>