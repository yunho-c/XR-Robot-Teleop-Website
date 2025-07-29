<script>
let { children } = $props();
</script>

<header class="copy px-4 md:px-8">
  <h1 class="text-3xl text-opacity-50">{@render children()}</h1>
</header>
