<script>
	import Email from './Email.svelte'


	let step = 0;
	
	const stepComponents = [Email]


	</script>

<form>	
	<svelte:component this={stepComponents[step]}/>
</form>