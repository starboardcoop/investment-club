<script>
    export let inset;
</script>

<div class="px-2 md:px-4 py-4 mx-auto w-full md:w-3/4 lg:w-2/3 max-w-5xl" class:inset>
    <slot></slot>
</div>

<style lang="postcss">
    .inset {
        @apply px-4 md:px-8;
    }
</style>