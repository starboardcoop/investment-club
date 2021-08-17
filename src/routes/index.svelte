<script>
    import Column from '$lib/Column.svelte'
    import Input from '$lib/Input.svelte'
    import Row from '$lib/Row.svelte';
    import Button from '$lib/Button.svelte';
    import Grid from '$lib/Grid.svelte'

    const interestRate = 0.1;
    const calculateEarnings = (contribution) => Number(contribution) * 12 * interestRate;
    let potentialEarnings = calculateEarnings(20); 
</script>

<Column>
    <h1>We're a co-op that invests in co-ops.</h1>
    <Grid>
        <Column>
            <p>With a monthly investment to a local co-operative, you can grow your money while supporting sustainable business.</p>
        </Column>
        <Column>
            <Input on:input={event => potentialEarnings = calculateEarnings(event.target.value)} label="Monthly Contribution:" placeholder="20 - 200"/>
            <div class="flex flex-col gap-2">
                <div class="pl-1 text-gray-500 text-sm">Potential Annual Earnings</div>
                <h1>$ {potentialEarnings}</h1>
            </div>
        </Column>
    </Grid>
</Column>
