<script>
  import { onMount } from "svelte";
  import linksData from "../config/links";
  import Links from "../components/Links.svelte";

  let links = [];
  onMount(() => (links= linksData));
</script>

<svelte:head>
	<title>Link</title>
</svelte:head>

<div>
  <h1 class="text-center mb-4 text-4xl">リンク</h1>
</div>

<div class="flex justify-center container">
  <Links {links} />
</div>