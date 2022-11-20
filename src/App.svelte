<script>
    import Home from "./pages/Home.svelte";
    import Project from "./pages/Project.svelte";
    import NotFound from "./pages/NotFound.svelte";
    import { Router, Route, Link } from "svelte-routing";
    import Uses from "./pages/Uses.svelte";

    export let url = "";
</script>

<div class="router">
  <Router url="{url}">
    <ul>
      <li><Link to="/">Home</Link></li>
      <li><Link to="projects">Project</Link></li>
      <li><Link to="uses">Uses</Link></li>
      <li><a href="">Source Code</a></li>
    </ul>
    <div>
     <Route path="/"><Home /></Route>
     <Route path="projects" component="{Project}" />
     <Route path="uses" component="{Uses}"></Route>
    </div>
    <Route component="{NotFound}" />
  </Router>
</div>

<style>
:global(a) {
    color: #4FD1C5;
}

ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
  overflow: hidden;
  position: -webkit-sticky; /* Safari */
  position: sticky;
  top: 0;
  background-color: #181A1B;
}
li {
  float: left;
}

li :global(a) {
    display: block;
    text-align: center;
    padding: 10px 10px;
    text-decoration: none;
}

li :global(a):hover {
  background-color: #111;
}

:root {
    font-family: "Iosevka Web";
    color: #E8E6E3;
    background-color: #181A1B;
    text-decoration: none;
}

@font-face {
	font-family: 'Iosevka Web';
	font-display: swap;
	font-weight: 400;
	font-stretch: normal;
	font-style: normal;
	src: url('./ttf/iosevka-regular.ttf') format('truetype'), url('./woff2/iosevka-regular.woff2') format('woff2');
}
</style>
