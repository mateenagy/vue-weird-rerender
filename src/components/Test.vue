<script lang="ts" setup>
import { onBeforeUnmount } from 'vue';

const props = defineProps<{
	name: string;
}>();

onBeforeUnmount(() => {
	console.log('[name]: ', props.name);
})
</script>
<template>
	<div>{{ name }}</div>
</template>
