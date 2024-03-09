<script>
    import Header from "../components/Header.svelte";
    import "../app.css";
</script>

<main>
    <Header/>
    <div class="flex justify-center items-center">
        <hr class="hr-dashed">
    </div>
    <slot />
</main>