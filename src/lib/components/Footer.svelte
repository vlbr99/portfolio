<script>
  let { className } = $props();
  export { className as class };
  import { Box } from "lucide-svelte";
</script>

<footer class={className}>
  <a href="/" class="logo"><Box size={32} /></a>
  <nav class="footer_nav">
    <ul>
      <li>
        <a target="_blank" href="https://whirra.vercel.app">Powered by Whirra</a
        >
      </li>
    </ul>
  </nav>
</footer>

<style>
  footer {
    background-color: #99ffe4;
    background-image: radial-gradient(
        at 91% 94%,
        rgb(37, 230, 162) 0px,
        transparent 50%
      ),
      radial-gradient(at 37% 37%, hsla(203, 97%, 62%, 1) 0px, transparent 50%),
      radial-gradient(at 27% 96%, rgb(143, 243, 113) 0px, transparent 50%);
    background-attachment: fixed;
    padding: 15px;
    width: 100%;
    display: flex;
    align-items: center;
    justify-content: space-between;
  }

  .logo {
    font-weight: bold;
    color: var(--primary_color_dark);
  }

  .footer_nav ul {
    display: flex;
    list-style-type: none;
  }

  .footer_nav li {
    list-style-type: none;
    margin-left: 10px;
  }

  .footer_nav a {
    color: var(--primary_color_dark);
    text-decoration: none;
    transition: 0.3s;
  }

  .footer_nav a:hover {
    color: rgb(41, 41, 41);
  }

  @media (max-width: 768px) {
  }
</style>
