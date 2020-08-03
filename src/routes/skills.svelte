<script>
  import { onMount } from "svelte";
  import skillsData from "../config/skills";
  import Skills from "../components/Skills.svelte";

  let skills = [];
  onMount(() => (skills= skillsData));
</script>

<svelte:head>
	<title>Skill</title>
</svelte:head>

<div>
  <h1 class="text-center mb-4 text-4xl">スキル</h1>
</div>

<div class="flex justify-center container">
  <Skills {skills} />
</div>