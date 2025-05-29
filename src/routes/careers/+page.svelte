<script lang="ts">
	// Types

	// Components
	import SectionHeader from "$lib/components/layout/SectionHeader.svelte";
	import Culture from "$lib/components/layout/Culture.svelte";
	import Testimonials from "$lib/components/layout/Testimonials.svelte";
	import SecondaryHero from "$lib/components/layout/hero-sections/SecondaryHero.svelte";
	import Card from "$lib/components/ui/Card.svelte";
	import JobList, { type JobOpening } from "./JobList.svelte";

	// Icons
	import IconBriefcase from "~icons/lucide/briefcase";
	import IconUsers from "~icons/lucide/users";
	import IconHeart from "~icons/lucide/heart";
	import IconGlobe from "~icons/lucide/globe";

	// Constants
	const SECTION_BASE_CLASSES = "section-py section-px container mx-auto";
	const GRADIENT_BG_CLASSES =
		"bg-gradient-to-br from-gray-50 to-gray-100 dark:from-gray-900 dark:to-gray-800";
	const ICON_CONTAINER_CLASSES =
		"bg-primary-50 text-primary-600 dark:bg-primary-950 dark:text-primary-400 flex items-center justify-center rounded-full";

	const benefits = [
  {
    title: "Build real-world AI",
    description:
      "Work on embodied AI and VLAM tech that is changing how entire industries operate — with impact you can see in the real world.",
    icon: IconBriefcase
  },
  {
    title: "Growth without ceiling",
    description:
      "Flat hierarchies, direct access to leadership, and opportunities to shape strategy and tech from day one.",
    icon: IconUsers
  },
  {
    title: "Flexible, meaningful work",
    description:
      "Flexible location and hours, modern Berlin/Potsdam offices, and a collaborative, supportive team from top universities and companies.",
    icon: IconHeart
  }
];

	const openings: JobOpening[] = [
		// Engineering
		{
			title: "Senior Frontend Developer",
			department: "Engineering",
			location: "Remote",
			type: "Full-time",
			url: "#"
		},
		{
			title: "Backend Engineer",
			department: "Engineering",
			location: "Remote",
			type: "Full-time",
			url: "#"
		},
		{
			title: "Design Engineer",
			department: "Engineering",
			location: "Remote",
			type: "Full-time",
			url: "#"
		},

		// Design
		{
			title: "UX/UI Designer",
			department: "Design",
			location: "Remote",
			type: "Full-time",
			url: "#"
		},
		{
			title: "Product Designer",
			department: "Design",
			location: "Remote",
			type: "Full-time",
			url: "#"
		},

		// Product
		{
			title: "Product Manager",
			department: "Product",
			location: "Remote",
			type: "Full-time",
			url: "#"
		},
		{
			title: "Product Analyst",
			department: "Product",
			location: "Remote",
			type: "Full-time",
			url: "#"
		},

		// Marketing
		{
			title: "Marketing Specialist",
			department: "Marketing",
			location: "Remote",
			type: "Full-time",
			url: "#"
		},
		{
			title: "Content Strategist",
			department: "Marketing",
			location: "Remote",
			type: "Full-time",
			url: "#"
		},
		{
			title: "Social Media Manager",
			department: "Marketing",
			location: "Remote",
			type: "Full-time",
			url: "#"
		}
	];

	const employeeTestimonials = [
  {
    name: "Sophia Zhang",
    position: "Robotics Engineer",
    company: "Engineering Team",
    quote:
      "I’ve never worked somewhere I felt so welcomed and empowered. Every idea counts, and my team celebrates our differences as strengths.",
    image: "/generated/image-a-professional-headshot-of-a-smiling-fem.webp"
  },
  {
    name: "Omar Khalil",
    position: "Product Manager",
    company: "Product Team",
    quote:
      "There are real opportunities to grow here — I’ve had mentors champion me and the trust to take on big projects from day one. The feedback and support are constant.",
    image: "/generated/image-a-professional-headshot-of-a-middle-east.webp"
  },
  {
    name: "Alex Rivera",
    position: "Senior Operations Specialist",
    company: "Operations",
    quote:
      "The environment is dynamic but everyone’s voice is heard. I feel respected and can truly shape how we work together as a team.",
    image: "/generated/image-a-professional-headshot-of-a-non-binary-.webp"
  }
];

	const processSteps = [
  {
    step: 1,
    title: "Apply online",
    description:
      "Send your CV (or LinkedIn) and a few lines on why sensmore excites you. Every application is reviewed by a real person."
  },
  {
    step: 2,
    title: "Intro call",
    description:
      "A short call to get to know each other, share your story, and answer any burning questions."
  },
  {
    step: 3,
    title: "Role deep dive",
    description:
      "Interview or challenge tailored to your field. We look for practical skills and how you solve real problems."
  },
  {
    step: 4,
    title: "Meet the team",
    description:
      "Connect with founders and future teammates, and get a sense of sensmore’s working style and culture."
  },
  {
    step: 5,
    title: "Offer & feedback",
    description:
      "We move quickly (usually within a week). You’ll get clear feedback and a transparent offer, plus space for all your questions."
  }
];

	const values = [
  {
    icon: IconHeart,
    title: "Builders, not spectators",
    description: "We work hands-on and take ownership, whether we’re solving field challenges or building new prototypes."
  },
  {
    icon: IconUsers,
    title: "Courage & curiosity",
    description: "We welcome hard questions and encourage experimentation. Curiosity and bold ideas drive our progress."
  },
  {
    icon: IconGlobe,
    title: "Grit in every environment",
    description: "From the lab to the mine, we build for reality and thrive in messy, tough situations."
  },
  {
    icon: IconBriefcase,
    title: "Voices heard",
    description: "Good ideas win. Everyone can influence big decisions—regardless of role or background."
  },
  {
    icon: IconHeart,
    title: "Diversity & belonging",
    description: "We support each other, celebrate differences, and know that varied perspectives make our team stronger."
  }
];
</script>

<!-- Hero Section -->

<SecondaryHero
	title="Advance embodied AI. Transform heavy industry."
	subtitle="Join world-class minds. Build real-world impact that scales."
	imageSrc="/generated/image-a-diverse-team-of-engineers-collaboratin.webp"
/>

<!-- Why Join Us Section -->
<section class={SECTION_BASE_CLASSES}>
	<SectionHeader title="Why join us?" subtitle="Build your career while making an impact" />

	<div class="mt-16 grid gap-4 md:grid-cols-3">
		{#each benefits as benefit}
			<Card {...benefit} />
		{/each}
	</div>
</section>

<!-- Culture Section -->
<Culture {values} />

<Testimonials testimonials={employeeTestimonials} />

<!-- Application Process -->
<section class={SECTION_BASE_CLASSES}>
	<div class="mx-auto">
		<h2 class="text-title1 mb-16">Our application process</h2>

		<div class="grid gap-12 md:grid-cols-3">
			{#each processSteps as { step, title, description }, i}
				<div class="flex flex-col">
					<div class="{ICON_CONTAINER_CLASSES} mb-6 size-11">
						<span class="text-headline">{step}</span>
					</div>
					<h3 class="text-headline mb-3">{title}</h3>
					<p class="text-body text-emphasis-low">{description}</p>
				</div>
			{/each}
		</div>
	</div>
</section>
<!-- Current Openings Section -->
<section class={GRADIENT_BG_CLASSES}>
	<div class="section-px section-py container mx-auto grid w-full items-start lg:grid-cols-2">
		<SectionHeader title="Current openings" subtitle="Find your perfect role" />

		<JobList {openings} />
	</div>
</section>
