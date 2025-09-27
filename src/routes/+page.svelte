<script lang="ts">
	// Components
	import Summary from "$lib/components/layout/Summary.svelte";
	import Features from "$lib/components/layout/Features.svelte";
	import Testimonials from "$lib/components/layout/Testimonials.svelte";
	import CallToAction from "$lib/components/layout/CallToAction.svelte";
	import AboutTeaser from "$lib/components/layout/AboutTeaser.svelte";
	import LogoScroller from "$lib/components/layout/LogoScroller.svelte";
	import Hero from "$lib/components/layout/hero-sections/Hero.svelte";
</script>

<Hero
	title="Find music that finds you"
	subtitle="Real shows. Local artists. No algorithms."
	imageSrc="/generated/image-a-small-group-of-young-adults-aged-22-35.webp"
	centered={false}
/>
<LogoScroller 
	label="Trusted by music lovers everywhere"
	logoUrls={[
		'https://cdn.brandfetch.io/spotify.com/w/400/h/400/logo',
		'https://cdn.brandfetch.io/airbnb.com/w/400/h/400/logo',
		'https://cdn.brandfetch.io/soundcloud.com/w/400/h/400/logo',
		'https://cdn.brandfetch.io/redbull.com/w/400/h/400/logo'
	]}
/>

<Summary
	generating
	title="What we do"
	text="Our technology delivers measurable results through secure, adaptable solutions that directly increase productivity and drive growth."
/>

<Testimonials
	testimonials={[
		{
			name: "Rhea Mendez",
			position: "Talent buyer",
			company: "Loose Clubroom, Austin",
			quote:
				"I used to check five different pages to find good shows. Now I just wait for my Thursday drop.",
			image: "/generated/image-a-professional-headshot-of-a-young-latin.webp"
		},
		{
			name: "Micah Lomax",
			position: "Event lead",
			company: "Basement Sessions, Chicago",
			quote:
				"We doubled attendance in one month without spending a dime on promo—we just let our local tastemaker do the talking.",
			image: "/generated/image-a-professional-headshot-of-a-young-black.webp"
		},
		{
			name: "Dakari Yen",
			position: "Music enthusiast",
			company: "Brooklyn",
			quote:
				"It cuts the noise. I don't have to dig—just follow people I trust and Showpass does the rest.",
			image: "/generated/image-a-professional-headshot-of-a-young-asian.webp"
		}
	]}
/>

<Features
	title="Discover music that moves you"
	subtitle="Skip the algorithms and find your next favorite artist through curated local experiences"
	features={[
		{
			title: "Curated weekly picks",
			description: "Local tastemakers handpick the best shows each week, eliminating discovery paralysis with trusted recommendations that match your taste.",
			imageSrc: "/generated/image-a-candid-editorial-style-image-of-young-.webp"
		},
		{
			title: "Location-based matching",
			description: "Find intimate venues and emerging artists within walking distance of your neighborhood using smart proximity matching.",
			imageSrc: "/generated/image-a-documentary-style-photograph-inside-an.webp"
		},
		{
			title: "Direct artist connections",
			description: "Skip the middleman and connect directly with local musicians, building authentic relationships that go beyond streaming.",
			imageSrc: "/generated/image-a-warm-moody-photograph-of-an-intimate-l.webp"
		},
		{
			title: "Real-time availability",
			description: "See live ticket availability and venue capacity instantly, ensuring you never miss out on intimate shows that sell out fast."
		},
		{
			title: "College venue network",
			description: "Access exclusive shows at university venues and student-run spaces that mainstream platforms overlook."
		},
		{
			title: "Authentic experiences",
			description: "Discover hidden gems and underground venues where real music culture happens, far from commercial algorithms."
		}
	]}
/>
<AboutTeaser generating />
<CallToAction generating />
