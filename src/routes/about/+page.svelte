<script lang="ts">
	// Components
	import CallToAction from "$lib/components/layout/CallToAction.svelte";

	// Icons
	import StakeholderGrid from "$lib/components/layout/StakeholderGrid.svelte";
	import Story from "./Story.svelte";
	import SecondaryHero from "$lib/components/layout/hero-sections/SecondaryHero.svelte";
	import Culture from "$lib/components/layout/Culture.svelte";

	// Constants
	const values = [
		{
			title: "Authenticity",
			description: "We champion real artists and genuine musical experiences over manufactured popularity."
		},
		{
			title: "Community",
			description: "Local music scenes are the heartbeat of culture—we exist to strengthen these connections."
		},
		{
			title: "Discovery",
			description: "Every music lover deserves to find their next favorite artist before everyone else does."
		}
	];
</script>

<SecondaryHero
	title="Find music that finds you"
	subtitle="Real shows. Local artists. No algorithms."
	imageSrc="/generated/image-a-group-of-young-music-founders-aged-22-.webp"
/>

<!-- Story Section -->
<Story
	paragraphs={[
		"Niclas and Chloe started this company because they were tired of missing incredible shows happening right in their neighborhood. Despite living in vibrant music cities, they kept discovering amazing local artists only after their intimate venue shows had already sold out.",
		"The problem wasn't lack of talent—it was discovery. Mainstream algorithms pushed the same popular acts while hidden gems performed to half-empty rooms just blocks away. Music lovers craved authentic experiences, but finding them felt impossible.",
		"We believe music discovery should feel personal, not algorithmic. Real artists deserve real audiences, and music lovers deserve to find shows that genuinely move them. That's why we built a platform that connects hearts, not just data points.",
		"Our mission goes beyond ticket sales—we're rebuilding the bridge between artists and their communities. When local venues thrive and artists find their people, the entire music ecosystem gets stronger. That's the future we're working toward, one show at a time."
	]}
/>

<!-- Our Culture Section -->
<Culture {values} />

<!-- StakeholderGrid Section -->
<StakeholderGrid
	stakeholderType="team"
	title="Meet the founders"
	subtitle="Passionate music lovers building the future of discovery"
	stakeholders={[
		{
			name: "Niclas Heussinger",
			position: "Chief Executive Officer",
			bio: "Music enthusiast who believes every great artist deserves to find their audience, and every music lover deserves to discover their next favorite band.",
			image: "https://www.unc.mn/image-placeholder.svg"
		},
		{
			name: "Chloe Smith",
			position: "Chief Marketing Officer",
			bio: "Community builder with deep roots in local music scenes, dedicated to connecting artists with the fans who will love them most.",
			image: "https://www.unc.mn/image-placeholder.svg"
		}
	]}
/>

<StakeholderGrid
	stakeholderType="investor"
	title="Backed by the best"
	subtitle="Point Nine, TSIC and others"
	stakeholders={[
		{
			name: "Point Nine Capital",
			image: "https://cdn.brandfetch.io/pointnine.com/w/400/h/400/logo?c=1id_elLz2Bd5Ej-dWo7"
		},
		{
			name: "TSIC Ventures",
			image: "https://cdn.brandfetch.io/tiny.vc/w/400/h/400/logo?c=1a2b3c4d5e"
		},
		{
			name: "Sequoia Capital",
			image: "https://cdn.brandfetch.io/sequoiacap.com/w/400/h/400/logo"
		}
	]}
/>

<!-- CTA Section -->
<CallToAction
	title="Ready to discover?"
	subtitle="Your next favorite show is waiting"
	description="Join music lovers who've discovered their new favorite artists through intimate venue experiences that you'll never find on mainstream platforms."
/>
