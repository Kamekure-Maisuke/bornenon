<script>
  export let skills;
</script>

<table class="table-auto">
  <tbody>
    {#each skills as skill }
    <tr>
      <td class="border px-4 py-2">{skill.category}</td>
      <td class="border px-4 py-2">{skill.type}</td>
    </tr>
    {/each}
  </tbody>
</table>