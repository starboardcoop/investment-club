<script>
    import Column from '$lib/Column.svelte';
    import Grid from '$lib/Grid.svelte';
    import Calculator from '$lib/Calculator.svelte';
    import { Anchor, Dollar, Users } from '$lib/icons';
</script>

<Column>
    <div class="flex flex-col space-y-4 mb-16">
        <h1 class="md:w-2/3">We're starting a co-op that invests in co-ops.</h1>
        <Grid>
            <Column>
                <p class="text-2xl">With a recurring monthly contribution to our investment club, you could grow your money while building the next economy.</p>
            </Column>
            <Calculator />
        </Grid>
    </div>
    <h2 class="mb-16">Why a cooperative investment club?</h2>
    <div class="grid grid-cols-1 md:grid-cols-3 gap-x-4 gap-y-24">
        <div class="flex flex-row justify-center items-center text-green-400"><Anchor /></div>
        <div class="md:col-span-2">
            <p>Our co-op investment club will only invest in Rhode island cooperative business. This puts money back into Rhode Island, instead of sucking it out of the state.</p>
        </div>

        <div class="flex flex-row justify-center items-center text-green-400"><Dollar /></div>
        <div class="md:col-span-2 flex flex-col space-y-4">
            <p>Big banks put their money where they think the can get the biggest returns. They also tend to ignore people who don’t already have a lot of money. You probably want your money to be used for socially useful purposes.</p>
            <p>As a member of our co-op investment club, you get a say in which ventures are good investments for our community.</p>
        </div>

        <div class="flex flex-row justify-center items-center text-green-400"><Users /></div>
        <div class="md:col-span-2 flex flex-col space-y-4">
            <p>Even though a traditional local business keeps money and jobs in Rhode Island, its top-down structure means that the people at the top get most of the benefit.</p>
            <p>Cooperatives more fairly distribute profits and responsibilities. They also tend to be more sustainable, so money invested in them has a better chance of getting paid back.</p>
        </div>
    </div>
</Column>