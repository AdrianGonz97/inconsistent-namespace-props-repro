<script lang="ts">
	import * as Button from "$lib";
</script>

<!-- See completions with CTRL+SPACE (or CMD+SPACE on MacOS I _think_) -->


<!-- === Cases where completions _WORK_ as expected === -->

<!-- When the prop doesn't contain an expression 
					 👇						-->
<Button.Root disabled >Works</Button.Root>

<!-- When the component is self closing 
		    👇								-->
<Button.Root />




<!-- === Cases where completions _DO NOT work_ as expected === -->

<!-- When there are no props already present 
		    👇								-->
<Button.Root >Doesn't Work</Button.Root>

<!-- After props with expressions 
						    👇				-->
<Button.Root disabled={true} >Doesn't Work</Button.Root>

<!-- When the completion is triggered between 
	the component name and the first prop 
	        👇								-->
<Button.Root  disabled={true}>Doesn't Work</Button.Root>
