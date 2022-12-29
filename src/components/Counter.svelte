<script>
  let count = 0
  const increment = () => {
    count += 1
  }
  $: double = count * 2

  $: {
    console.log(`現在のcountの値は${count}です`);
    console.log('複数行も設定できます。');
  }
</script>

<button on:click={increment}>
  count is {count}
  double is {double}

{#if count<5}
  countは5未満です
{:else}
  countは5以上です
{/if}
</button>
