<script>
	export let name;

	let count = 0;

	$: doubled = count + 1;
	
	function handleClick() {
		count += 1;
		name = 'Rickhy';
	}
</script>

<button on:click={handleClick}>
	Click
</button>

<p>Hello {name} </p>
<p>Clicked: {doubled} </p>