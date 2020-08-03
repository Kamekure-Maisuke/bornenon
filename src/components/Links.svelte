<script>
  export let links;
</script>

<table class="table-auto">
  <tbody>
    {#each links as link }
    <tr>
      <td class="border px-4 py-2">
        <a
          href={link.url}
          target="_blank" rel="noopener noreferrer"
          class="no-underline hover:underline text-blue-500 text-lg"
        >
          {link.name}
        </a>
      </td>
    </tr>
    {/each}
  </tbody>
</table>