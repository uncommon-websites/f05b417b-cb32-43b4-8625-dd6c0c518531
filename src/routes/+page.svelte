<script lang="ts">
	// Components
	import UseCases from "$lib/components/layout/UseCases.svelte";
	import Summary from "$lib/components/layout/Summary.svelte";
	import Features from "$lib/components/layout/Features.svelte";
	import Testimonials from "$lib/components/layout/Testimonials.svelte";
	import CallToAction from "$lib/components/layout/CallToAction.svelte";
	import AboutTeaser from "$lib/components/layout/AboutTeaser.svelte";
	import LogoScroller from "$lib/components/layout/LogoScroller.svelte";
	import CustomerCardHero from "$lib/components/layout/hero-sections/CustomerCardHero.svelte";
</script>

<CustomerCardHero
  centered={true}
  title="Trusted by teams built for the toughest work"
  subtitle="sensmore partners with leaders in mining, construction, defense, and agriculture to keep critical machinery running—safely, efficiently, and without interruption."
  customers={[
    {
      name: "CEMEX",
      position: "Quarry operations manager",
      imageSrc: "/generated/image-a-female-mining-manager-standing-confide.webp",
      quote: "With sensmore’s technology, our loaders operate smoothly even in the worst weather—keeping throughput steady and teams safe."
    },
    {
      name: "Harrington Construction",
      position: "Construction supervisor",
      imageSrc: "/generated/image-a-male-construction-site-supervisor-stan.webp",
      quote: "Installing Machine Assist across machines simplified our safety process—reducing downtime and increasing site coordination."
    },
    {
      name: "Paus",
      position: "Defense site engineer",
      imageSrc: "/generated/image-a-female-engineer-in-the-defense-industr.webp",
      quote: "In underground defense sites, communication is mission critical. sensmore connects people and machines when it matters most."
    },
    {
      name: "AgriWorks Co.",
      position: "Head of agricultural operations",
      imageSrc: "/generated/image-a-male-leader-in-agricultural-operations.webp",
      quote: "Before sensmore, visibility on crops and carriers was our blind spot. Now we work with precision, day or night."
    },
    {
      name: "Lhoist",
      position: "Executive, mining operations",
      imageSrc: "/generated/image-a-female-mining-executive-is-seated-in-a.webp",
      quote: "The real-time site visibility has changed how we manage operations. It’s cleaner, faster, and decisions happen on the ground."
    }
  ]}
/>

<LogoScroller
	label="Trusted by industry leaders"
	logoUrls={[
		'https://logo.clearbit.com/bhp.com',
		'https://logo.clearbit.com/cat.com',
		'https://logo.clearbit.com/cemex.com'
	]}
/>

<Summary
	generating
	title="What we do"
	text="Our technology delivers measurable results through secure, adaptable solutions that directly increase productivity and drive growth."
/>




<Features
	generating
	title="Features"
	subtitle="Some features"
	features={[
		{
			title: "Streamlined Workflows",
			description:
				"Automate repetitive tasks and connect systems to improve productivity with our industry-leading 87% time savings."
		},
		{
			title: "Data Analysis",
			description:
				"Extract meaningful insights from your data with powerful analytical tools backed by proprietary AI algorithms that are 3x more accurate than competitors."
		},
		{
			title: "Secure Collaboration",
			description:
				"Work together seamlessly while maintaining strict data privacy standards with our zero-knowledge architecture and military-grade encryption."
		}
	]}
/>

<UseCases
	generating
	title="Use Cases"
	subtitle="Real-world applications for your business needs"
	useCases={[
		{
			title: "Streamlined Workflows",
			description:
				"Automate repetitive tasks and connect systems to improve productivity with our industry-leading 87% time savings.",
			image:
				"https://images.unsplash.com/photo-1552664730-d307ca884978?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=2940&q=80",
			link: {
				href: "/use-cases/workflows",
				label: "Learn more"
			}
		},
		{
			title: "Data Analysis",
			description:
				"Extract meaningful insights from your data with powerful analytical tools backed by proprietary AI algorithms that are 3x more accurate than competitors.",
			image:
				"https://images.unsplash.com/photo-1573496359142-b8d87734a5a2?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=2488&q=80",
			link: {
				href: "/use-cases/data-analysis",
				label: "Explore analytics"
			}
		},
		{
			title: "Secure Collaboration",
			description:
				"Work together seamlessly while maintaining strict data privacy standards with our zero-knowledge architecture and military-grade encryption.",
			image:
				"https://images.unsplash.com/photo-1522202176988-66273c2fd55f?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=2940&q=80",
			link: {
				href: "/use-cases/collaboration",
				label: "See security features"
			}
		}
	]}
/>

<AboutTeaser generating />
<CallToAction generating />
