<script>
    export let smallColumns = "1";
    export let mediumColumns = "2"; 
    export let largeColumns = "2";

    const smallColumnsStyle = () => {
        switch (smallColumns) {
            case "1":
            default:
                return "grid-cols-1"
        }
    }

    const mediumColumnsStyle = () => {
        switch (mediumColumns) {
            case "2":
            default:
                return "md:grid-cols-2"
        }
    }

    const largeColumnsStyle = () => {
        switch (largeColumns) {
            case "2":
            default:
                return "lg:grid-cols-2"
        }
    }
</script>

<div class="grid gap-4 {smallColumnsStyle()} {mediumColumnsStyle()} {largeColumnsStyle()}">
    <slot></slot>
</div>