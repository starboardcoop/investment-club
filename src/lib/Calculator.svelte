<script>
    import Column from "$lib/Column.svelte";
    import Row from "$lib/Row.svelte";

    const styles = {
        normal: "bg-gray-200 bg-opacity-10 hover:bg-opacity-25 active:ring-2 active:ring-green-300",
        selected: "bg-green-500 hover:bg-opacity-80"
    };

    const options = [
        {
            dollars: 20
        },
        {
            dollars: 50
        },
        {
            dollars: 100
        },
        {
            dollars: 200
        }
    ];

    let selected = 1;
    let annualFundraising = options[selected].dollars * 12;

    function calculate(option, index) {
        annualFundraising = option.dollars * 12;
        selected = index;
    }
</script>

<Column>
    <div class="flex flex-col gap-2">
        <div class="pl-1 text-gray-500 text-sm">Monthly Contribution</div>
        <Row>
            {#each options as option, i}
                <button on:click={() => calculate(option, i)} class="px-4 py-2 rounded font-semibold transform duration-100 {i === selected ? styles.selected : styles.normal}">${option.dollars}</button>
            {/each}
        </Row>
    </div>
    <div class="flex flex-col gap-2">
        <div class="pl-1 text-gray-500 text-sm">Annual Funding</div>
        <h1>$ {annualFundraising}</h1>
    </div>
</Column>