<!-- This is the FORM for each Item -->
<script>
  export let index;
  import ItemContent from "./ItemContent.svelte";
  import { toc } from "./toc.js";

  let item,
    bg = "";
  item = toc[index];
  if (item.thumbnail)
    bg =
      "bg-no-repeat bg-right-bottom bg-[url('/assets/" + item.thumbnail + "')]";
</script>

<style>
</style>

<!-- If item is FEATURED -->
{#if item.featured}
<div class="mb-5 bg-slate-700 rounded-lg h-[280px] {bg}">
  <ItemContent index={index} />
</div>

<!-- If item is UPDATED but NOT featured -->
{:else if item.updated}
<div class="w-full mb-5 bg-slate-700 rounded-lg h-[280px] {bg}">
  <ItemContent index={index} />
</div>

<!-- All other items -->
{:else}
<div class="w-full mb-5 border-2 border-slate-500 rounded-lg h-[280px]">
  <ItemContent index={index} />
</div>

{/if}