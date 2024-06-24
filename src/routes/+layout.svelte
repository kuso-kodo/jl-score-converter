<script>
	import '../app.css';
	import beams from '$lib/images/beams.jpg';
	import grid from '$lib/images/grid.svg';
</script>

<div class="app">
	<div class="relative flex min-h-screen flex-col justify-center overflow-hidden bg-gray-50 py-6 sm:py-12">
		<img src={beams} alt="" class="absolute left-1/2 top-1/2 max-w-none -translate-x-1/2 -translate-y-1/2" width="1308" />
		<div
			class="layout-grid absolute inset-0 bg-center [mask-image:linear-gradient(180deg,white,rgba(255,255,255,0))]"
			style:background-image="url({grid})"
		></div>
		<div class="relative bg-white px-6 pb-8 pt-10 shadow-xl ring-1 ring-gray-900/5 sm:mx-auto sm:max-w-lg sm:rounded-lg sm:px-10">
		  <div class="mx-auto max-w-md">
			<slot />
		  </div>
		</div>
	  </div>	  
</div>
