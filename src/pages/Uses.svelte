<script>
    import Typewriter from "svelte-typewriter/Typewriter.svelte";
     
    import Rust from "./posts/Rust.svelte";
    import Bevy from "./posts/Bevy.svelte";
    import Svelte from "./posts/Svelte.svelte";
    import IDE from "./posts/IDE.svelte";
    import Keyboard from "./posts/Keyboard.svelte";
    import Computer from "./posts/Computer.svelte";
    import Mouse from "./posts/Mouse.svelte";
    import Yew from "./posts/Yew.svelte";
</script>

<Typewriter>
    <h3 class="title">A list of tools I use on the daily</h3>
</Typewriter>

<h3 class="text">As a developper I spend hours on my computer trying to put code together so everyting can work (This only applies for weekends I have a life). For that I 
need the best technologies and the best workflow. So I've always being working on improving it by using tools such as tyling window managers. So I think it would be a nice 
idea to show you my tools and workflow.</h3>

<div class="grid-container">
  <div class="rust"><Rust /></div>
  <div class="bevy"><Bevy /></div>
  <div class="svelte"><Svelte /></div>  
  <div class="yew"><Yew /></div>
  <div class="computer"><Computer /></div>
  <div class="ide"><IDE /></div>
  <div class="keyboard"><Keyboard /></div>
  <div class="mouse"><Mouse /></div>
</div>

<style>
.grid-container {
    display: grid;
    grid-template-columns: auto auto auto;
    margin: auto;
    justify-content: center;
    gap: 20px;
}
.title {
    color: white;
    font-size: 25px; 
    text-decoration: underline;
    padding-left: 10px;
    text-align: center;
}

.text {
    display: block;
    margin-left: auto;
    margin-right: auto;
    width: 55%;
    text-align: center;
}

.keyboard {
    grid-row-start: 3;
    grid-row-end: 3;
    grid-column-start: 1;
    grid-column-end: 1;
}

.mouse {
    grid-row-start: 3;
    grid-row-end: 3;
    grid-column-start: 3;
    grid-column-end: 3;
}
</style>
