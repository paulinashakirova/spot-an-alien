<template>
  <div class='modal'>
<h3 v-if="uiState === 'win'">Congrats! You won!</h3>
<h3 v-else-if="uiState === 'lose'">Loser, you lost!</h3>
<p v-else>lol</p>
  </div>
</template>

<script>
import { mapState } from 'vuex';
  export default {
    computed: {
		...mapState(['uiState'])
	},
  }
</script>



<style lang="scss" scoped> </style>
