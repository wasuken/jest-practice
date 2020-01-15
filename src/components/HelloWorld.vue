<template>
	<div class="count">
		<h1>This is an count page</h1>
		{{$store.state.count}}
		<button @click="increment">+</button>
		<button @click="decrement">-</button>
	</div>
</template>

<script>
 import { mapMutations } from "vuex";
 export default {
	 name: 'HelloWorld',
	 methods: mapMutations(["increment", "decrement"]),
 };
</script>
