<script>
	import "./styles.css";
	export let name, age;

	$: uppercaseName = name.toUpperCase();

	function changeName() {
		name = prompt();
	}
</script>

<div class="hayo">
	<div class="title-container">
		<h1>
			Hello {uppercaseName} and {age + 1}!
		</h1>
	</div>
	<div class="button-container">
		<button on:click={changeName}>Change Name</button>
	</div>
</div>
