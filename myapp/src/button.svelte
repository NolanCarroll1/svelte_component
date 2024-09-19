<script>
  export let name = "Default";
  export let type = "disabled"; // regular, flat, disabled
  export let size = "md"; // sm, md, lg
  export let color = "purple";
  const sizes = {
    sm: "px-1 py-3 pr-8 pl-8",
    md: "px-5 py-3 pr-8 pl-8",
    lg: "px-7 py-5 pr-8 pl-8",
  };
</script>

{#if type == "regular"}
  <button
    class={`rounded-full bg-${color}-600 hover:bg-blue-500 font-bold text-gray-200 ${size in sizes ? sizes[size] : sizes["md"]}`}
  >
    {name}
  </button>
{/if}

{#if type == "flat"}
  <button
    class={`rounded-full font-bold border border-2 border-none text-${color}-600 ${size in sizes ? sizes[size] : sizes["md"]}`}
  >
    {name}
  </button>
{/if}

{#if type == "disabled"}
  <button
    class={`rounded-full font-bold border border-2 border-gray-700 text-gray-700 ${size in sizes ? sizes[size] : sizes["md"]}`}
  >
    {name}
  </button>
{/if}
