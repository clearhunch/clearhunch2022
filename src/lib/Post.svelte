<script>
	export let image;
	export let title;
	export let description;
</script>

<div class="flex items-center w-full mt-8">
	<div class="h-48 w-48 rounded-xl overflow-hidden">
		<img class="object-cover w-full h-full" src={image} alt="Blog Header" />
	</div>
	<div class="ml-6 flex-1">
		<h3 class="text-blue-600 text-2xl font-bold">{title}</h3>
		<p class="text-gray-600 mt-3 mb-1 max-w-screen-sm">
			{description}
		</p>
		<a href="#" class="text-blue-600 underline"> Read More </a>
	</div>
</div>
