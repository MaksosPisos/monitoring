<script>
  import LocomotiveScroll from "locomotive-scroll";
  import "locomotive-scroll/dist/locomotive-scroll.min.css";
  import Chart from "chart.js/auto";
  import colors from "tailwindcss/colors";
  import { onMount } from "svelte";
  // import Header from "./components/Header.svelte";
  // import Charts from "./components/Charts.svelte";
  import Footer from "./components/Footer.svelte";
  import Main from "./components/Main.svelte";

  // скролл
  function createScroll() {
    const scroll = new LocomotiveScroll({
      el: document.querySelector("[data-scroll-container]"),
      smooth: true,
    });
    scroll.on("call", (e) => {
      if (e === "chartCall") {
        console.log("chartCall");
      }
      if (e === "pieCall") {
        console.log("pieCall");
      }
    });
  }
  onMount(createScroll);

  //theme
  let toogleCheck;
  let themeDefault = "";
  if (
    localStorage.getItem("theme") === "winter" ||
    localStorage.getItem("theme") === null
  ) {
    toogleCheck = false;
    themeDefault = "winter";
  } else if (localStorage.getItem("theme") === "dracula") {
    toogleCheck = true;
    themeDefault = "dracula";
  }

  function switchTheme() {
    if (themeDefault === "winter") {
      toogleCheck = true;
      themeDefault = "dracula";
      localStorage.setItem("theme", "dracula");
    } else {
      toogleCheck = false;
      themeDefault = "winter";
      localStorage.setItem("theme", "winter");
    }
  }
</script>

<div data-scroll-container data-theme={themeDefault} class=" transition-all">
  <div class=" max-w-[1400px] mx-auto">
    <div class="navbar bg-base-300 fixed z-[100] max-w-[1400px] mx-auto">
      <div class="navbar-start">
        <div class="dropdown">
          <label tabindex="0" class="btn btn-ghost btn-circle">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              class="h-5 w-5"
              fill="none"
              viewBox="0 0 24 24"
              stroke="currentColor"
              ><path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M4 6h16M4 12h16M4 18h7"
              /></svg
            >
          </label>
          <ul tabindex="0" class="menu menu-compact dropdown-content mt-3 p-2 shadow bg-base-100 rounded-box w-52"          >
            <li><a href="/">Homepage</a></li>
            <li><a href="/">Portfolio</a></li>
            <li><a href="/">About</a></li>
          </ul>
        </div>
    </div>
      <div class="navbar-center">
        <a class="btn btn-ghost normal-case text-xl" href="/">daisyUI</a>
      </div>
      <div class="navbar-end">
        <div class="form-control">
          <label class="label cursor-pointer">
            <input
              type="checkbox"
              class="toggle toggle-primary"
              on:click={switchTheme}
              checked={toogleCheck}
            />
          </label>
        </div>
      </div>
    </div>
  </div>
  <Main />

  <Footer />
</div>
