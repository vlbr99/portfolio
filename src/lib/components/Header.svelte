<script>
  let { className } = $props();
  export { className as class };
  import { Box } from "lucide-svelte";
</script>

<header class={className}>
  <nav>
    <div class="logo">
      <a href="/"><Box size={36} /></a>
    </div>
  </nav>
</header>

<style>
  header {
    position: sticky;
    top: 0;
    width: 100%;
    background-color: var(--primary_color_dark);
    z-index: 1;
    text-decoration: none;
    list-style-type: none !important;
  }
  header nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 20px;
  }
  header nav #menu-toggle {
    display: none;
  }
  header nav #menu-toggle:checked ~ .menu {
    transform: scale(1, 1);
  }
  header nav .menu {
    display: flex;
    justify-content: center;
    align-items: flex-start;
  }
  header nav .menu li {
    list-style-type: none;
  }
  header nav .menu a {
    display: block;
    padding: 7px 15px;
    font-weight: 500;
    color: var(--light_touch_color_dark);
    text-decoration: none;
    transition: 0.3s;
  }
  header nav .menu a:hover {
    color: white;
  }
  header .logo a {
    font-weight: bold;
    text-decoration: none;
    font-size: 1.8rem;
    color: var(--secondary_color_dark);
  }
  header .menu-icon {
    background-color: transparent !important;
    color: transparent;
  }
  @media only screen and (max-width: 950px) {
    .menu {
      flex-direction: column;
      background-color: var(--touch_color_dark);
      align-items: flex-start;
      position: absolute;
      top: 70px;
      left: 0;
      width: 100%;
      z-index: 1;
      transform: scale(1, 0);
      transform-origin: top;
      transition: transform 0.3s ease-in-out;
    }
    .menu a {
      margin-left: 15px;
    }
    .menu li {
      margin-bottom: 10px;
    }
    .menu-icon {
      display: block;
      color: var(--secondary_color_dark) !important;
      font-size: 28px;
      cursor: pointer;
      background-color: var(--secondary_color_dark) !important;
    }
  }
</style>
