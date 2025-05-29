<script lang="ts">
	// Types
	import type { PageProps } from "./$types";

	// Components
	import Features from "$lib/components/layout/Features.svelte";
	import Testimonials from "$lib/components/layout/Testimonials.svelte";
	import CallToAction from "$lib/components/layout/CallToAction.svelte";
	import Pricing from "$lib/components/layout/Pricing.svelte";

	// Props
	const { data }: PageProps = $props();
</script>

<Pricing />

<Testimonials
  testimonials={[
    {
      name: "Clara Weiss",
      position: "Head of Quarry Operations",
      company: "Lhoist Group",
      quote: "Within weeks of deployment, sensmore cut our site’s near-misses by over 80%. That kind of impact made the investment a no-brainer.",
      image: "/generated/image-a-professional-headshot-of-clara-weiss-a.webp"
    },
    {
      name: "Cem Gürsel",
      position: "Safety & Automation Lead",
      company: "CEMEX Europe",
      quote: "No cables, no winter fog breakdowns. sensmore’s radar-based mapping just works and delivers clear ROI, even in tough weather.",
      image: "/generated/image-a-professional-headshot-of-cem-grsel-a-m.webp"
    },
    {
      name: "Emil Lindström",
      position: "Mining Technology Advisor",
      company: "Paus GmbH",
      quote: "I’ve worked with a lot of site tech. Nothing else integrates this fast—and keeps everyone aligned from day one.",
      image: "/generated/image-a-professional-headshot-of-emil-lindstrm.webp"
    }
  ]}
/>

<CallToAction
  title="Ready for safer, smarter operations?"
  subtitle="See sensmore in action on your site"
  description="Join the teams leading the industry with AI-driven heavy machinery. Boost productivity, keep your crew safe, and gain live control from pit to plant. See how real customers turn downtime into results–even in the harshest conditions."
  imageSrc="/generated/image-a-cheerful-mining-site-manager-standing-.webp"
  callsToAction={[
    { href: "/contact", label: "Request a demo", variant: "primary" },
    { href: "/contact", label: "Talk to an expert", variant: "secondary" }
  ]}
/>
