<template>
    <button
        type="button"
        class="inline-flex relative items-center justify-center w-8 h-8 focus:outline-none focus:ring rounded-lg"
    >
        <span :class="{ invisible: processing || loading }">
            <slot />
            <Icon v-if="icon" :name="icon" type="solid" />
        </span>

        <span
            v-if="processing || loading"
            class="absolute"
            style="top: 50%; left: 50%; transform: translate(-50%, -50%)"
            >
            <Loader class="text-gray-500" width="32" />
        </span>
    </button>
</template>

<script>
    import { Icon } from "laravel-nova-ui";

    export default {
        components: { Icon },

        props: {
            icon: {
                type: String,
                required: false,
            },

            loading: {
                type: Boolean,
                default: false,
            },

            processing: {
                type: Boolean,
                default: false,
            },
        },
    }
</script>
