<script>
	import Step from '../components/Step.svelte';

	let steps = [
		{
			name: 'Project 1',
			href: 'https://yuppiecaronas.com.br',
			icon: 'fa-solid fa-code'
		},
		{
			name: 'Project 2',
			href: 'http://hasslefreecleaningservices.co.uk',
			icon: 'fa-solid fa-code'
		},
		{
			name: 'Project 3',
			href: '#',
			icon: 'fa-solid fa-code'
		}
	];

	// let benefits = [
	// 	{
	// 		metric: '10x',
	// 		name: 'a self taught developer',
	// 		description:
	// 			'I taught myself to code using free online resources and absolutely fell in love with the creativity and problem solving that is involved in developing and engineering innovative new online experiences. Starting of with JavaScript, HTML & CSS and evolving my knowledge base to include JavaScript frameworks, backend programming, design, cloud services and much much more.'
	// 	},
	// 	{
	// 		name: 'a product design & UX finatic',
	// 		description:
	// 			'Carefully crafting and designing amazing user experiences allows me to express and experiment with every morsel of creativity I have. I love the challenge of learning new design concepts and enabling users with amazing online experiences.'
	// 	},
	// 	{
	// 		name: 'an excellent communicator',
	// 		description:
	// 			"Communication is key and it's a paramount value of mine. I believe in transparency and constructive communication above all else. This helps me develop deep relationships and ensures my effectiveness and productivity in any work space with any team."
	// 	}
	// ];
</script>

<main class="flex flex-col flex-1 p-4">
	<section id="introPage" class="grid grid-cols-1 lg:grid-cols-2 gap-10 py-8 sm:py-14">
		<div class="flex flex-col text-center lg:justify- lg:text-left gap-6 md:gap-8 lg:gap-10">
			<h2 class="font-semibold text-4xl sm:text-5xl md:text-6xl">
				Hi! I'm <span class="poppins text-violet-400">João Pedro Cordeiro</span> Software Engineer
				based in <span class="text-violet-400">Brazil</span>.
			</h2>
			<p class="text-base sm:text-lg md:text-xl">
				My <span class="text-violet-400">favorite tech</span> includes Javascript (Next.JS or SvelteKit),
				TailwindCSS, Node.js and learning Go.
			</p>
			<a
				href="https://www.linkedin.com/in/joaopedrorc/"
				target="_blank"
				class="blueShadow mx-auto lg:mr-auto text-base sm:text-lg md:text-xl poppins relative overflow-hidden px-6 py-3 group rounded-full bg-white text-slate-950"
			>
				<div
					class="absolute top-0 right-full w-full h-full bg-violet-400 opacity-20 group-hover:translate-x-full z-0 duration-200"
				/>
				<h4 class="relative z-9">Get in touch &rarr;</h4>
			</a>
		</div>
		<div class="relative shadow-2xl grid place-items-center">
			<img src="" alt="" class="object-cover z-[2] max-h-[70vh]" />
		</div>
	</section>

	<section id="projects" class="py-20 lg:py-32 flex flex-col gap-24">
		<div class="flex flex-col gap-2 text-center">
			<h6 class="text-lg sm:text-xl md:text-2xl">A few of my creative endeavors</h6>
			<h3 class="text-3xl sm:text-4xl md:text-5xl font-semibold">
				Curious to <span class="poppins text-violet-400">see</span>
				my work?
			</h3>
		</div>

		<div class="grid grid-cols-1 lg:grid-cols-3 gap-12 lg:gap-10">
			<Step step={steps[0]}>
				<p>
					Project:
					<strong class="text-violet-400"
						>Car riding services exclusive for university students</strong
					>
					Founder of Yuppie Caronas Universitárias is a Brazilian startup that solves the problem of
					university students who need to commute to their universities and don't have a car.
				</p>
			</Step>

			<Step step={steps[1]}>
				<p>
					Project:
					<strong class="text-violet-400">Business Website WordPress + Next.JS</strong>
					Hassle-Free Cleaning Services is a UK based cleaning company that needed a website to showcase
					their services and allow customers to book appointments online.
				</p>
			</Step>

			<Step step={steps[2]}>
				<p>
					Project:
					<strong class="text-violet-400">Business Website React.Js + Node.JS and Express </strong>
					GGallery Painting and Decorating is a UK based painting and decorating company that needed
					a website to showcase their services and allow customers to book appointments online.
				</p>
			</Step>
		</div>
	</section>

	<!-- <section
		id="about"
		class="py-20 pt-10 lg:pt16 lg:py-32 flex flex-col gap-16 sm:gap-20 md:gap-24 relative"
	>
		<div
			class="flex flex-col gap-2 text-center relative before:absolute before:top-0 before:left-0 before:w-2/3 before:h-1.5 before:bg-violet-700 after:absolute after:bottom-0 after:right-0 after:w-2/3 after:h-1.5 after:bg-violet-700 py-4"
		>
			<h6 class="text-lg sm:text-xl md:text-2xl">Want to know more?</h6>
			<h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl">
				A bit <span class="poppins text-violet-400">about</span> me.
			</h3>
		</div>

		<p class="mx-auto poppins font-semibold text-lg sm:text-xl md:text-2xl">I am ...</p>
		<div class="flex flex-col gap-20 w-full mx-auto max-w-[800px]">
			{#each benefits as benefit, index}
				<div class="flex gap-6 sm:gap-8">
					<p class="poppins text-4xl sm:text-5xl md:text-6xl text-slate-500 font-semibold">
						0{index + 1}
					</p>
					<div class="flex flex-col gap-6 sm:gap-8">
						<h3 class="text-2xl sm:text-3xl md:text-5xl">
							{benefit.name}
						</h3>
						<p>{benefit.description}</p>
					</div>
				</div>
			{/each}
		</div>
	</section> -->
</main>
