# Svelte Syntax Highlighting Example

This file demonstrates Svelte syntax highlighting in markdown.

## Simple Component

```svelte
<script>
  let count = 0;

  function increment() {
    count += 1;
  }
</script>

<button on:click={increment}>
  Clicks: {count}
</button>

<style>
  button {
    background: #ff3e00;
    color: white;
    border: none;
    padding: 10px 20px;
    border-radius: 5px;
  }
</style>
```

## Component with Reactivity

```svelte
<script>
  let firstName = 'Svelte';
  let lastName = 'Developer';

  $: fullName = `${firstName} ${lastName}`;
</script>

<input bind:value={firstName} placeholder="First name" />
<input bind:value={lastName} placeholder="Last name" />

<p>Hello, {fullName}!</p>
```

## Component with Props

```svelte
<script>
  export let title = 'Default Title';
  export let items = [];
</script>

<h2>{title}</h2>

<ul>
  {#each items as item}
    <li>{item}</li>
  {/each}
</ul>
```

## JavaScript for Comparison

```javascript
const count = 0

function increment() {
  count += 1
}
```
