<script>
    export let type = "normal";
</script>

<button on:click {...$$props} class="px-4 py-2 rounded font-semibold transform duration-100 {type}">
    <slot></slot>
</button>

<style lang="postcss">
    .normal {
        @apply bg-gray-200 bg-opacity-10 hover:bg-opacity-25;
        @apply active:bg-opacity-100 active:ring-2 active:ring-gray-300;
    }

    .primary {
        @apply bg-green-500 hover:bg-opacity-25;
        @apply active:bg-opacity-100 active:ring-2 active:ring-green-300;
    }

    .ghost {
        @apply bg-gray-200 bg-opacity-0 hover:bg-opacity-10;
        @apply active:bg-opacity-80 active:ring-2 active:ring-gray-300;
    }

    .danger {
        @apply bg-red-200 bg-opacity-10 hover:bg-opacity-25;
        @apply active:bg-opacity-100 active:ring-2 active:ring-red-300;
    }
</style>