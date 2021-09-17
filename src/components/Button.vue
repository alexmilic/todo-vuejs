<template>
    <button 
        @click="onClick()"
        :style="{backgroundColor: color}"
        class="btn"
    >
        {{ text }}
    </button>
</template>

<script lang="ts">
export default {
    name: 'Button',
    props: {
        text: {
            type: String,
            default: 'Add task'
        },
        color: {
            type: String,
            color: "#ccc"
        }
    },
    methods: {
        onClick() {
            console.log('clicked');
        }
    }
}
</script>