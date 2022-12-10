<script>
    import Header from "./Header.svelte";
    import Content from "./Content.svelte"
</script>
<section>
    <!-- <div class="circle"></div> -->
    <Header />
    <Content />
    
</section>

<style>

    :root {
        background: linear-gradient(#f3ec78, #af4261);
    }

    * {
        margin: 0;
        padding: 0;
        box-sizing: border-box;

        
    }

    section {
        position: relative;
        width: 100%;
        min-height: 98vh;
        padding: 100px;
        display: flex;
        justify-content: space-between;
        align-items: center;
        
    }
    
    .circle {
        position: absolute;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        background-image: linear-gradient(45deg, #f3ec78, #af4261);
        clip-path: circle(800px at right bottom);
    }
</style>