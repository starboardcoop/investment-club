<script>
    export let justify = "left";
    export let align = "center";
    export let inset;

    const justifyStyle = () => {
        switch (justify) {
            case "between":
                return "justify-between";
            case "right":
                return "justify-end";
            case "left":
            default:
                return "justify-start";
        }
    }

    const alignStyle = () => {
        switch (align) {
            case "top":
                return "items-start";
            case "center":
            default:
                return "items-center";
        }
    }
</script>

<div class="flex flex-row gap-4 {justifyStyle()} {alignStyle()}" class:inset>
    <slot></slot>
</div>

<style>
    .inset {
        @apply p-4;
    }
</style>