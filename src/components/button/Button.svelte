<script>
  export let disabled = false;
  export let active = false;
  export let onClick;
</script>

<button
  class={`
    bg-black border-black border-4 rounded h-12 px-4 mx-2 text-lg 
    ${active ? 'highlight-gray' : ''} 
    hover:highlight-white
    merged-middle:join merged-first:join-first merged-last:join-last
    disabled:disabled
  `}
  disabled={disabled}
  on:click={onClick}
>
  <slot></slot>
</button>