<script lang="ts">
	import SectionHeader from "$lib/components/layout/SectionHeader.svelte";
	import { animate, stagger } from "motion";
	import { onMount } from "svelte";

	// Types
	export type Value = {
		title: string;
		description: string;
	};

	// Props
	const { values = [] }: { values: Value[] } = $props();

	let cards: HTMLElement[] = $state([]);

	onMount(() => {
		if (!cards.length) return;
		animate(
			cards,
			{
				y: ["1.5rem", 0],
				filter: ["blur(2px)", "blur(0px)"],
				opacity: [0, 1]
			},
			{
				duration: 0.3,
				ease: "easeOut",
				delay: stagger(0.1, {
					ease: "easeInOut"
				})
			}
		);
	});
</script>

<section class="bg-white dark:bg-gray-950">
	<div
		class="section-py section-px container mx-auto grid gap-8 [--gap:--spacing(8)] [--radius:var(--radius-2xl)]"
	>
		<SectionHeader title="How we work together." subtitle="Five values that drive sensmore forward" />

  <div class="grid lg:grid-cols-5 gap-(--gap)">
    <div class="row-span-2 col-span-1 lg:col-span-2 flex flex-col items-center justify-center">
      <img src="/generated/image-a-diverse-team-of-people-from-different-.webp" alt="The sensmore team working together in an industrial setting" class="rounded-xl w-full object-cover aspect-[3/4] mb-6 lg:mb-0"/>
    </div>
    <div class="col-span-1 lg:col-span-3 grid gap-(--gap)">
      {#each values as value, i}
        <div
          bind:this={cards[i]}
          class="relative border-t border-gray-200 pt-4 dark:border-gray-900"
        >
          <!-- Content -->
          <div class="text-caption z-10">
            <div>
              <div class="text-headline mb-[1em]">{value.title}</div>
              <div class="text-body text-gray-500 dark:text-gray-400">{value.description}</div>
            </div>
          </div>
        </div>
      {/each}
    </div>
  </div>
	</div>
</section>
