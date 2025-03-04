<script>
  import "../routes/index.scss";
  import svelte_img from "../lib/assets/svelte.png";
  import css from "../lib/assets/css.png";
  import js from "../lib/assets/js.png";
  import scss from "../lib/assets/scss.png";
  import vercel from "../lib/assets/logo-vercel-svgrepo-com.svg";
  import git from "../lib/assets/git.png";
  import github from "../lib/assets/gh.png";
  import mongoose from "../lib/assets/mongodb-svgrepo-com.svg";
  import whirra from "../lib/assets/whirra.png";
  import figma from "../lib/assets/figma.png";
  import { Shell } from "lucide-svelte";
</script>

<div class="about_wrapper">
  <div class="about_wraper_about_me">
    <div class="about_me">
      <div class="pfp"></div>
      <div class="my_data">
        <p>Velibor Minić</p>
        <p>Bosnia and Herzegovina</p>
        <p>Full Stack Web Developer</p>
      </div>
    </div>
    <div class="description">
      <p>
        I'm a passionate web developer with 5 years of experience, always coding
        something new. Addicted to problem-solving, I develop fast while keeping
        code clean and maintainable. My stack includes Svelte, Mongoose,
        JavaScript, and SCSS, but I'm always open to learning. With a strong
        grasp of internet technologies, I build secure and efficient apps.
        Fluent in English, I collaborate well and stay updated with trends.
        Whether it's a new idea or an optimization challenge, I love turning
        concepts into high-performance solutions. Let's build something great!
      </p>
    </div>
  </div>
</div>
<div class="stack_wrapper">
  <h1>Tools I Use Daily</h1>
  <div class="tools_wrapper">
    <div class="tools_row">
      <div class="svelte">
        <img src={svelte_img} alt="svelte" />
        <p>SvelteKit</p>
      </div>
      <div class="js">
        <img src={js} alt="js" />
        <p>JavaScript</p>
      </div>
      <div class="css">
        <img src={css} alt="css" />
        <p>CSS</p>
      </div>
      <div class="scss">
        <img src={scss} alt="scss" />
        <p>SCSS</p>
      </div>
      <div class="scss">
        <img src={figma} alt="figma" />
        <p>Figma</p>
      </div>
    </div>
    <div class="tools_row">
      <div class="mongoose">
        <img src={mongoose} alt="mongoose" />
        <p>Mongoose</p>
      </div>
      <div class="vercel">
        <img src={vercel} alt="vercel" />
        <p>Vercel</p>
      </div>
      <div class="git">
        <img src={git} alt="git" />
        <p>Git</p>
      </div>
      <div class="github">
        <img src={github} alt="gh" />
        <p>Github</p>
      </div>
      <div class="github">
        <Shell />
        <p>Whirra</p>
      </div>
    </div>
  </div>
</div>
<div class="projects_wrapper">
  <h1>MY LATEST PROJECTS</h1>
  <div class="projects">
    <div class="project_row">
      <div>
        <img src={whirra} alt="whirra" />
        <main class="project_text">
          <h2>Whirra</h2>
          <p>
            A SvelteKit + Mongoose multitool designed to accelerate website
            development.
          </p>
          <main class="project_buttons">
            <a href="#">Github</a>
            <a href="#">whirra.vercel.app</a>
          </main>
        </main>
      </div>
      <div>
        <img src={whirra} alt="whirra" />
        <main class="project_text">
          <h2>Whirra</h2>
          <p>
            A SvelteKit + Mongoose multitool designed to accelerate website
            development.
          </p>
          <main class="project_buttons">
            <a href="#">Github</a>
            <a href="#">whirra.vercel.app</a>
          </main>
        </main>
      </div>
    </div>
    <div class="project_row">
      <div>
        <img src={whirra} alt="whirra" />
        <main class="project_text">
          <h2>Whirra</h2>
          <p>
            A SvelteKit + Mongoose multitool designed to accelerate website
            development.
          </p>
          <main class="project_buttons">
            <a href="#">Github</a>
            <a href="#">whirra.vercel.app</a>
          </main>
        </main>
      </div>
      <div>
        <img src={whirra} alt="whirra" />
        <main class="project_text">
          <h2>Whirra</h2>
          <p>
            A SvelteKit + Mongoose multitool designed to accelerate website
            development.
          </p>
          <main class="project_buttons">
            <a href="#">Github</a>
            <a href="#">whirra.vercel.app</a>
          </main>
        </main>
      </div>
    </div>
  </div>
</div>
<div class="contact">
  <h1>LET'S BRING YOUR IDEAS TO LIFE</h1>
  <a href="mailto:velibordev@gmail.com" target="_blank">velibordev@gmail.com</a>
</div>
