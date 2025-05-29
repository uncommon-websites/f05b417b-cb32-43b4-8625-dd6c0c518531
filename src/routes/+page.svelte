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
	title="What we do"
	text="sensmore brings intelligent automation to the world’s toughest machines. Our embodied AI platform makes heavy equipment smarter, safer, and ready for any challenge—across mining, construction, defense, and agriculture."
/>




<Features
  title="Smarter machines for the real world"
  subtitle="AI-driven features designed for harsh work environments"
  features={[
    {
      title: "Embodied AI for heavy machinery",
      description: "Physical AI and VLAM bring human-like intelligence to your loaders, dozers, and haulers."
    },
    {
      title: "4D radar and vision fusion",
      description: "Reliable, all-weather detection that sees through rain, fog, dust, and darkness."
    },
    {
      title: "Real-time digital twin",
      description: "Live site mapping and terrain updates keep your operations precise, productive, and safe."
    },
    {
      title: "Rapid retrofit & integration",
      description: "Modular hardware and software install on existing fleets—no rip and replace needed."
    },
    {
      title: "Safer, smarter operations",
      description: "Prevent accidents with real-time collision alerts, zone management, and situational awareness."
    },
    {
      title: "Zero-shot loader automation",
      description: "Fully autonomous material handling adapts instantly to changing environments—no manual retraining."
    }
  ]}
/>

<UseCases
	title="Use Cases"
	subtitle="Real-world applications for your business needs"
	useCases={[
		{
			title: "Prevent unplanned downtime",
			description: "Continuous monitoring of equipment health and site activity spots problems early—stopping costly failures before they start.",
			image: "/generated/image-a-heavy-mining-loader-with-workers-navig.webp",
			link: {
				href: "/use-cases/equipment-health-monitoring",
				label: "See how it works"
			}
		},
		{
			title: "Operate safely in any condition",
			description: "AI-powered loaders and assists keep machines and teams protected with collision alerts and situational awareness—even in fog, dust, or darkness.",
			image: "/generated/image-a-construction-loader-operating-in-low-v.webp",
			link: {
				href: "/use-cases/safe-all-weather-operation",
				label: "Learn more"
			}
		},
		{
			title: "Gain visibility, manage more site",
			description: "Live site mapping and real-time insights let you track every truck, loader, and material flow from one dashboard—no matter the scale.",
			image: "/generated/image-a-group-of-engineers-gathered-outdoors-a.webp",
			link: {
				href: "/use-cases/live-site-visibility",
				label: "See live dashboard"
			}
		}
	]}
/>

<Testimonials
  testimonials={[
    {
      name: "Malik Tenner",
      position: "Pit Supervisor",
      company: "Raxon Minerals",
      quote: "Planning and dispatch that used to take me 3 hours a day now takes 30 minutes because of the live insights from Site OS. That's time I can spend solving bigger problems.",
      image: "/generated/image-a-male-mining-supervisor-stands-confiden.webp"
    },
    {
      name: "Liesa Walcott",
      position: "Fleet Safety Lead",
      company: "RegenField Construction",
      quote: "Before sensmore Machine Assist, we averaged two vehicle-related incidents a month. We've now gone five months without a single one—and that’s through every weather curveball.",
      image: "/generated/image-a-female-construction-fleet-safety-lead-.webp"
    },
    {
      name: "Hagen Blix",
      position: "Operations Director",
      company: "Norholm Resources",
      quote: "We saved over €180,000 in the first quarter alone by reducing unplanned crusher stoppages. Just seeing boulders before they break things makes all the difference.",
      image: "/generated/image-a-male-mining-operations-director-stands.webp"
    }
  ]}
/>

<AboutTeaser />
<CallToAction
  title="Smarter machines. Safer sites."
  subtitle="Start your transformation"
  description="Connect with sensmore to reduce risk, cut downtime, and get full visibility—directly from the machines you already run."
  imageSrc="/generated/image-a-cheerful-mining-industry-manager-stand.webp"
  callsToAction={[{ href: '/contact', label: 'Connect with us', variant: 'primary' }]}
/>
