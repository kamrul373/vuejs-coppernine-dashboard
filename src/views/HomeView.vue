/* eslint-disable */
<template>
  <div class="home">
    <HomeSidebar />
    <HomeFeed />
  </div>
</template>

<script>
import { defineComponent } from 'vue'
import HomeSidebar from '../components/HomeSidebar.vue'
import HomeFeed from '@/components/HomeFeed.vue'

export default defineComponent({
	name: 'HomeView',
	components: {
		HomeSidebar,
		HomeFeed
	}
})
</script>
<style>
.home {
	display: flex;
	column-gap: 20px;
}

@media all and (max-width: 768px) {
	.home {
		flex-direction: column-reverse
	}
}
</style>
