<script>
	//@ts-ignore
	import SvelteTooltip from 'svelte-tooltip';

	import { ChevronLeft, ChevronRight, Search } from 'lucide-svelte';
</script>

<div class="flex jc:space-between ai:center">
	<div>Latest Requests</div>

	<div class="flex gap:25 min-w:50% jc:flex-end">
		<input
			type="text"
			name="search"
			id="search"
			placeholder="Search for a request"
			class="p:15 r:10 b:1|solid|gray-80 min-w:50%"
		/>

		<button
			class="bg:black bg:gray-90:hover cursor:pointer p:10 r:10 w:50px"
		>
			<SvelteTooltip tip="My Items" color="#FFF" bottom>
				<Search color="#FFF" />
			</SvelteTooltip>
		</button>
	</div>
</div>

<div class="grid grid-cols:2@sm grid-cols:3@md gap:25">
	<div
		class="flex flex:col gap:20 w:full b:1|solid|black r:10 px:25 py:20 bg:gray-95 h:full"
	>
		<h2>ID Card</h2>
		<p class="fg:gray-40">
			Lorem ipsum dolor, sit amet consectetur adipisicing elit. Laudantium
			cumque eveniet aperiam facere culpa nulla est dignissimos! Dolor cum
			voluptatem ullam itaque distinctio, modi earum quo error alias
			dolorem obcaecati.
		</p>

		<span><strong>Lost near: </strong> SJT </span>
	</div>

	<div
		class="flex flex:col gap:20 w:full b:1|solid|black r:10 px:25 py:20 bg:gray-95 h:full"
	>
		<h2>ID Card</h2>
		<p class="fg:gray-40">
			Lorem ipsum dolor, sit amet consectetur adipisicing elit. Laudantium
			cumque eveniet aperiam facere culpa nulla est dignissimos! Dolor cum
			voluptatem ullam itaque distinctio, modi earum quo error alias
			dolorem obcaecati.
		</p>

		<span><strong>Lost near: </strong> SJT </span>
	</div>

	<div
		class="flex flex:col gap:20 w:full b:1|solid|black r:10 px:25 py:20 bg:gray-95 h:full"
	>
		<h2>ID Card</h2>
		<p class="fg:gray-40">
			Lorem ipsum dolor, sit amet consectetur adipisicing elit. Laudantium
			cumque eveniet aperiam facere culpa nulla est dignissimos! Dolor cum
			voluptatem ullam itaque distinctio, modi earum quo error alias
			dolorem obcaecati.
		</p>

		<span><strong>Lost near: </strong> SJT </span>
	</div>

	<div
		class="flex flex:col gap:20 w:full b:1|solid|black r:10 px:25 py:20 bg:gray-95 h:full"
	>
		<h2>ID Card</h2>
		<p class="fg:gray-40">
			Lorem ipsum dolor, sit amet consectetur adipisicing elit. Laudantium
			cumque eveniet aperiam facere culpa nulla est dignissimos! Dolor cum
			voluptatem ullam itaque distinctio, modi earum quo error alias
			dolorem obcaecati.
		</p>

		<span><strong>Lost near: </strong> SJT </span>
	</div>

	<div
		class="flex flex:col gap:20 w:full b:1|solid|black r:10 px:25 py:20 bg:gray-95 h:full"
	>
		<h2>ID Card</h2>
		<p class="fg:gray-40">
			Lorem ipsum dolor, sit amet consectetur adipisicing elit. Laudantium
			cumque eveniet aperiam facere culpa nulla est dignissimos! Dolor cum
			voluptatem ullam itaque distinctio, modi earum quo error alias
			dolorem obcaecati.
		</p>

		<span><strong>Lost near: </strong> SJT </span>
	</div>

	<div
		class="flex flex:col gap:20 w:full b:1|solid|black r:10 px:25 py:20 bg:gray-95 h:full"
	>
		<h2>ID Card</h2>
		<p class="fg:gray-40">
			Lorem ipsum dolor, sit amet consectetur adipisicing elit. Laudantium
			cumque eveniet aperiam facere culpa nulla est dignissimos! Dolor cum
			voluptatem ullam itaque distinctio, modi earum quo error alias
			dolorem obcaecati.
		</p>

		<span><strong>Lost near: </strong> SJT </span>
	</div>

	<div
		class="flex flex:col gap:20 w:full b:1|solid|black r:10 px:25 py:20 bg:gray-95 h:full"
	>
		<h2>ID Card</h2>
		<p class="fg:gray-40">
			Lorem ipsum dolor, sit amet consectetur adipisicing elit. Laudantium
			cumque eveniet aperiam facere culpa nulla est dignissimos! Dolor cum
			voluptatem ullam itaque distinctio, modi earum quo error alias
			dolorem obcaecati.
		</p>

		<span><strong>Lost near: </strong> SJT </span>
	</div>

	<div
		class="flex flex:col gap:20 w:full b:1|solid|black r:10 px:25 py:20 bg:gray-95 h:full"
	>
		<h2>ID Card</h2>
		<p class="fg:gray-40">
			Lorem ipsum dolor, sit amet consectetur adipisicing elit. Laudantium
			cumque eveniet aperiam facere culpa nulla est dignissimos! Dolor cum
			voluptatem ullam itaque distinctio, modi earum quo error alias
			dolorem obcaecati.
		</p>

		<span><strong>Lost near: </strong> SJT </span>
	</div>

	<div
		class="flex flex:col gap:20 w:full b:1|solid|black r:10 px:25 py:20 bg:gray-95 h:full"
	>
		<h2>ID Card</h2>
		<p class="fg:gray-40">
			Lorem ipsum dolor, sit amet consectetur adipisicing elit. Laudantium
			cumque eveniet aperiam facere culpa nulla est dignissimos! Dolor cum
			voluptatem ullam itaque distinctio, modi earum quo error alias
			dolorem obcaecati.
		</p>

		<span><strong>Lost near: </strong> SJT </span>
	</div>
</div>

<div class="flex jc:flex-end ai:center gap:25">
	<span>Showing results 1 - 9 of 500</span>

	<div>
		<button
			class="bg:black bg:gray-90:hover cursor:pointer p:10 r:10 w:50px"
		>
			<SvelteTooltip tip="My Items" color="#FFF" bottom>
				<ChevronLeft color="#FFF" />
			</SvelteTooltip>
		</button>

		<button
			class="bg:black bg:gray-90:hover cursor:pointer p:10 r:10 w:50px"
		>
			<SvelteTooltip tip="My Items" color="#FFF" bottom>
				<ChevronRight color="#FFF" />
			</SvelteTooltip>
		</button>
	</div>
</div>
