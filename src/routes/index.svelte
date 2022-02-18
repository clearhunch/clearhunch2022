<script context="module" lang="ts">
	export const prerender = true;
</script>

<script lang="ts">
	import Post from '$lib/Post.svelte';
	const data = [
		{
			title: 'Nitty Gritty: Building a Svelte Blog',
			description:
				'The infamous first command line of starting a project. I was sitting on a Sunny in mid-feburary deciding between which command to run to kick off my new personal site. The...',
			image:
				'https://images.unsplash.com/photo-1517373116369-9bdb8cdc9f62?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=2070&q=80'
		},
		{
			title: 'Keeping 2022 Personal or: Why I built this blog.',
			description:
				'The infamous first command line of starting a project. I was sitting on a Sunny in mid-feburary deciding between which command to run to kick off my new personal site. The...',
			image:
				'https://images.unsplash.com/photo-1587654780291-39c9404d746b?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=2070&q=80'
		},
		{
			title: 'How I became a programmer.',
			description:
				'I started programming in 2007. I wouldn’t call me a good student. I would say that 99% of teachers would say I was a below average student...',
			image:
				'https://images.unsplash.com/photo-1587654780291-39c9404d746b?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=2070&q=80'
		}
	];
</script>

<svelte:head>
	<title>Home</title>
</svelte:head>

<section class="flex relative flex-nowrap items-start flex-row max-w-screen-xl mx-auto">
	<div class="flex items-start w-80 py-10 h-screen max-w-screen-md">
		<div class="border-r px-6 self-stretch">
			<div class="w-28 rounded-full overflow-hidden">
				<img src="profile.png" alt="My Memoji" class="w-full h-full" />
			</div>
			<h1 class="text-xl mt-4 mb-1 font-semibold">Christopher Edge</h1>
			<p class="text-gray-600">
				Senior Software Engineer <a href="https://zylo.com" class="text-blue-500">@zylo</a><br
					class="mb-2"
				/>A midwesterner who likes to build systems to help make people and companies successful.
			</p>
			<div class="px-4 pt-3 pb-4 rounded-xl bg-blue-100 mt-6">
				<p class="font-semibold">Get Article Updates</p>
				<p class="text-xs -mt-1">No spam ever. I promise.</p>
				<div class="relative">
					<input class="w-full mt-3 p-2 rounded" type="text" placeholder="i.montoya@tpb.com" />
					<svg
						xmlns="http://www.w3.org/2000/svg"
						class="absolute right-2 top-1/2 -mt-1 h-5 w-5 hover:text-blue-600 cursor-pointer"
						viewBox="0 0 20 20"
						fill="currentColor"
					>
						<path
							fill-rule="evenodd"
							d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-8.707l-3-3a1 1 0 00-1.414 1.414L10.586 9H7a1 1 0 100 2h3.586l-1.293 1.293a1 1 0 101.414 1.414l3-3a1 1 0 000-1.414z"
							clip-rule="evenodd"
						/>
					</svg>
				</div>
			</div>
			<p class="text-sm text-blue-500 mt-6">Feel free to borrow this blog's setup.</p>
		</div>
	</div>
	<div class="flex-1 w-full h-full">
		<div class="px-8 py-10">
			<h2 class="text-2xl font-bold">Recent Posts</h2>
			{#each data as story}
				<Post image={story.image} title={story.title} description={story.description} />
			{/each}
		</div>
	</div>
</section>
