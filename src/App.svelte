<script>
  import Counter from './components/Counter.svelte'
  import Text from './components/Text.svelte'
  const name = 'コンポーネント内で定義した変数'
  let bindName = 'aaa'
</script>

<main>
  <h1>Vite + Svelte</h1>

  <p>{name}</p>

  <div>
    <Text name="test1" />
    <Text name="test2" />
  </div>

  <div>
    <input type="text" bind:value={bindName} />
  </div>

  <div class="card">
    <Counter />
  </div>
</main>

<style>
</style>
