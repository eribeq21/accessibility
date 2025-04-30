<script>
	import '../app.css';
	let { children } = $props();
	
		const introduction = [
			{ text: "Welcome to Learn Accessibility!", link: "/learn/welcome" },
			{ text: "Aria & Html", link: "/learn/aria_html" },
			{ text: "Javascript", link: "/learn/javascript" },
			{ text: "Images", link: "/learn/images" }
		];
	
		let filterValue = $state("");
		let filteredResult = null;
	
		function filterFunction() {
			console.log("Filter value inside function:", filterValue); 
			filteredResult = introduction.find(item =>
				item.text.toLowerCase().includes(filterValue.toLowerCase())
			);
	
			if (filteredResult) {
				window.location.href = filteredResult.link;
			}
		}
	
	</script>
	
	<!-- Navbar -->
	<nav class="fixed top-0 left-0 z-30 w-full bg-white shadow-sm">
		<div class="flex items-center justify-between px-6 py-2 w-full">
			<!-- Left side: Logo -->
			<div class="flex items-center">
				<a href="/"><h1 class="text-2xl font-bold">
					<span class="text-blue-600">Learn</span>
					<span class="text-gray-800">with</span>
					<span class="text-green-500">Eriseldi</span>
				  </h1>
				</a>
			</div>
	
			<!-- Right side: Search + Buttons -->
			<div class="flex items-center gap-4">
				<!-- Search input -->
				<div class="relative">
				  <input
					bind:value={filterValue}
					type="text"
					placeholder="Search..."
					class="w-64 rounded-full border border-gray-300 py-1 pr-4 pl-10 text-gray-700 placeholder-gray-400 transition focus:border-transparent focus:ring-2 focus:ring-blue-400 focus:outline-none"
				  />
				 
				</div>
	
				<!-- Search button -->
				<button
				  class="rounded-full bg-blue-500 px-4 py-1 font-semibold text-white transition hover:bg-blue-600"
				  onclick={filterFunction}>
				  Visit
				</button>
			</div>
		</div>
	</nav>
	
	  {@render children()}
	
	
	