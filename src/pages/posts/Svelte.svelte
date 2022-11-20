<script>
    import img from "../../assets/svelte.png"
</script>

<div class="container">
    <img src={img} alt="Svelte" class="image">
    <h4 class="text">The Svelte JavaScript Framework</h4>
</div>

<style>
.container {
  display: grid;
  grid-template-columns: auto auto auto;
  gap: 10px;
}

.image {
    grid-row-start: 1;
    grid-row-end: 1;
    grid-column-start: 1;
    grid-column-end: 3;
    display: block;
    margin-left: auto;
    margin-right: auto;
    width: 300px;
    height: 150px;
    border-radius: 10px;
    padding: 0;
}

.text {
    grid-row-start: 2;
    grid-row-end: 2;
    grid-column-start: 1;
    grid-column-end: 3;
    text-align: center;
    padding: 0;
}
</style>
