<script lang="ts" setup>
import { ref } from 'vue';
import Test from './components/Test.vue'

const show = ref<boolean>(true);
</script>
<template>
	<div>
		<div>
			<span>When I remove foo the onBeforeUnmount event log `bar_bad`</span>
			<Test name="foo_bad" />
			<Test name="bar_bad" />
		</div>
		<!-- <div>
			<span>When I remove foo the onBeforeUnmount event log `foo_good`</span>
			<Test name="foo_good" />
			<div></div>
			<Test name="bar_good" />
		</div> -->
		<!-- <div>
			<span>When I remove foo the onBeforeUnmount event log `foo_good`</span>
			<Test name="foo_good" v-if="show" />
			<Test name="bar_good" />
		</div> -->
		<!-- <div>
			<span>When I remove foo the onBeforeUnmount event log `foo_good`</span>
			<div>
				<Test name="foo_good" />
			</div>
			<Test name="bar_good" />
		</div> -->
		<!-- <div>
			<span>When I remove foo the onBeforeUnmount event log `foo_good`</span>
			<Test name="foo_good" :key="Math.random()" />
			<Test name="bar_good" />
		</div> -->
	</div>
</template>
