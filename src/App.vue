<template>
	<div class="container">

		<div class="person_wrapper" v-for="person in persons" v-bind:key="person.id">
			<div><b>name: </b>{{person.name}}</div>
			<div><b>email: </b> {{person.email}} </div>
			<div><b>description: </b>{{person.desc}}</div>
		</div>

		<!-- counter -->
		
		<!-- <button @click="decrement">-</button>
		<h1>{{count}}</h1>
		<button @click="increment" >+</button> -->
	</div>
</template>

<script>
	export default {
		data() {
			return {
				persons: [
					{
						id: 1,
						name: "abdubosit",
						email: "abdubositjs@gmail.com",
						desc: "lorem ipsum dolor lorem ipsum dolor lorem ipsum dolor"
					},
					{
						id: 2,
						name: "nosir",
						email: "nosir5001@gmail.com",
						desc: "lorem ipsum dolor lorem ipsum dolor lorem ipsum dolor"
					},
					{
						id: 3,
						name: "abduvali",
						email: "abduvali@gmail.com",
						desc: "lorem ipsum dolor lorem ipsum dolor lorem ipsum dolor"
					}
				]
				// count: 0,
			}
		},
		methods: {
		
		
		
		/*	increment() {
				this.count += 1
			},
			decrement() {
				this.count -= 1
			}
		*/
		}
	}
</script>

<style>
	*{
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		font-family: sans-serif;
	}
	.container {
		padding: 50px;
		width: 100%;
		height: 100vh;
		background: rgb(180, 180, 255);
	}

	.person_wrapper {
		border: 1px solid gray;
		padding: 5px 10px;
		margin-bottom: 10px;
	}
	/* button {
		padding: 8px 24px;
		cursor: pointer;
		font-size: 20px;
		border: none;
		border-radius: 4px;
		
	}

	h1 {
		width: 100px;
		display: flex;
		justify-content: center;
		align-items: center;
	} */
</style>