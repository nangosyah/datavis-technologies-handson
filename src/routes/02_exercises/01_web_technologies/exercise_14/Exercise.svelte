<style>
	.btn-highlight {
		background-color: yellow;
	}
</style>

<script>
	let current = "";
	let lastClickedButton = null;
	
	function handleClick(buttonName, event) {
		current = buttonName;
		
		if (lastClickedButton) {
			lastClickedButton.classList.remove('btn-highlight');
		}
		
		event.target.classList.add('btn-highlight');
		lastClickedButton = event.target;
	}
</script>

<!-- We will cover buttons later on! -->
<button class="btn btn-secondary" on:click={(event) => handleClick("messi", event)}>
	Messi
</button>

<button class="btn btn-secondary" on:click={(event) => handleClick("ronaldo", event)}>
	Ronaldo
</button>

<button class="btn btn-secondary" on:click={(event) => handleClick("neymar", event)}>
	Neymar
</button>

