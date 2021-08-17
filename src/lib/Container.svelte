<script>
    export let inset;
</script>

<div class="px-4 py-4 mx-auto w-full md:w-3/4 lg:w-2/3 max-w-5xl" class:inset>
    <slot></slot>
</div>

<style>
    .inset {
        @apply px-8;
    }
</style>