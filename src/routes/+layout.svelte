<script>
  let { children } = $props();
  import Header from "../lib/components/Header.svelte";
  import Footer from "$lib/components/Footer.svelte";
  import "@fontsource-variable/geist";
  import favicon from "../lib/assets/favicon.ico";
</script>

<svelte:head>
  <link rel="icon" href={favicon} />
</svelte:head>

<Header></Header>
{@render children()}
<Footer></Footer>

<style>
  :global(:root) {
    --primary_color_dark: #000000;
    --secondary_color_dark: #ffffff;
    --light_touch_color_dark: #808080;
    --touch_color_dark: #161616;
    --secondary_touch_color_dark: #222222;
  }
  :global(*) {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: "Geist Variable", sans-serif;
  }
  :global(*::selection) {
    background-color: #042f2e !important;
    color: #2dd4bf;
  }
  :global(body) {
    background-color: var(--primary_color_dark);
    overflow-x: hidden;
    background-size: 80px 80px;
    background-image: linear-gradient(
        to right,
        rgb(10, 10, 10) 1px,
        transparent 1px
      ),
      linear-gradient(to bottom, rgb(10, 10, 10) 1px, transparent 1px);
  }
  :global(html) {
    overflow-x: hidden;
  }
</style>
