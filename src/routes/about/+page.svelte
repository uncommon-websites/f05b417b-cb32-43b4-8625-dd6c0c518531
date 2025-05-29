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
    title: "Operational resilience",
    description: "We engineer for the toughest environments—ensuring safety, reliability, and uptime, even when conditions turn harsh."
  },
  {
    title: "Hands-on innovation",
    description: "Our breakthroughs come from the field, not the lab—combining AI expertise with real-world grit."
  },
  {
    title: "Clarity in complexity",
    description: "We communicate transparently and prioritize action—making complex technologies understandable and practical for every operator."
  },
  {
    title: "Integrity, always",
    description: "Trust is built on openness, honesty, and respected commitments—to our partners, our team, and the safety of every worker."
  },
  {
    title: "Collaboration in every solution",
    description: "Great technology comes from working closely with the people who run, repair, and rely on heavy machinery every day."
  }
];
</script>

<SecondaryHero
	title="We build human-level intelligence into heavy machines"
	subtitle="Making mining, construction, and industrial sites safer, faster, and easier to run"
	imageSrc="/mockups/airport-screen-1748544611394.png"
/>

<!-- Story Section -->
<Story
	paragraphs={[
		"Every day, heavy machinery operates in environments where visibility is low, pressure is high, and mistakes can cost lives. Sites lose hours to downtime. Workers face real risks. Most machines still operate blindly. sensmore was founded to change that—to bring intelligence and awareness to the ground, where it matters most.",
		"Co-founders Bjarne Johannsen and Maximilian Rolf come from very different places: one deep in AI and robotics, the other immersed in industrial field work. They teamed up to tackle one of the biggest gaps in a hardware-heavy world—the missing layer of intelligence. With a team of experts from leading automotive and automation institutions, they launched sensmore with one goal: make machines act with awareness, not just automation.",
		"Today, sensmore powers safer, smarter operations in mining, construction, and beyond. From real-time operational views to autonomous loading and machine-level collision prevention, we reimagine how machines understand and act. Already trusted by forward-thinking partners like CEMEX, Lhoist, and Paus—our platform brings embodied AI and VLAM from theory into the field. Built by a world-class team. Backed by top investors. And always built to work when conditions get tough."
	]}
/>

<!-- Our Culture Section -->
<Culture {values} />

<!-- StakeholderGrid Section -->
<StakeholderGrid
  stakeholderType="team"
  title="Our founders."
  subtitle="Leadership made to deliver."
  stakeholders={[
    {
      name: "Bjarne Johannsen",
      position: "Co-founder & CTO",
      bio: "Bjarne draws on deep expertise in AI and robotics to lead sensmore's technology vision and product integrity. His work shapes how intelligence and autonomy scale in the harshest industrial environments.",
      image: "/generated/image-a-professional-headshot-of-a-founder-exu.webp"
    },
    {
      name: "Maximilian Rolf",
      position: "Co-founder & CEO",
      bio: "Maximilian combines hands-on field experience with a drive to modernize heavy industry. He guides sensmore’s mission to deliver practical impact—turning complex sites into smart, efficient operations.",
      image: "/generated/image-a-headshot-of-a-founder-capturing-confid.webp"
    }
  ]}
/>

<StakeholderGrid
  stakeholderType="investor"
  title="Backed by the best."
  subtitle="Investors: Point Nine, TSIC, Acequia Capital, Prototype Capital. Angels & advisors include Amar Shah, Arnoud Balhuizen, Michael Wax, Thilo Konzok, Roby Stancel, Robin Dechant, Alexey Zhigarev, and Elmar Leiblein."
  stakeholders={[
    {
      name: "Point Nine",
      image: "https://cdn.brandfetch.io/pointnine.com/w/400/h/400/logo?c=1id_elLz2Bd5Ej-dWo7"
    },
    {
      name: "TSIC",
      image: "https://cdn.brandfetch.io/tiny.vc/w/400/h/400/logo?c=1a2b3c4d5e"
    },
    {
      name: "Acequia Capital",
      image: "https://cdn.brandfetch.io/acequia.com/w/400/h/400/logo"
    },
    {
      name: "Prototype Capital",
      image: "https://cdn.brandfetch.io/prototype-capital.com/w/400/h/400/logo"
    }
  ]}
/>

<!-- CTA Section -->
<CallToAction
  title="Ready to shape the future of heavy industry?"
  subtitle="Partner with sensmore."
  description="We work with forward-thinking leaders who don’t settle for marginal gains. Whether you're looking to reduce downtime, increase safety, or take the next step toward autonomy—let's build it together.

Combine your site expertise with our AI-driven technology to create intelligent, reliable, and future-proof operations."
  imageSrc="/generated/image-a-diverse-team-of-people-from-different-.webp"
  callsToAction={[
    { href: "/contact", label: "Start a conversation", variant: "primary" },
    { href: "/platform", label: "See our platform", variant: "secondary" }
  ]}
/>
