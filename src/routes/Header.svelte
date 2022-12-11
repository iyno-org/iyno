<script>
    import logo from "$lib/images/brain.png"
</script>

<header>
    <a href="/" class="logo"><img src="{logo}" alt="logo">
    <div class="name">
        <h2 class="IYNO TEXT">IYNO</h2>
    </div>
    </a>
    <!-- <ul>
        <li><a href="/">Home</a></li>
        <li><a href="/journal">Journal</a></li>
        <li><a href="https://book.iyno.org">Book</a></li>
        <li><a href="/about">About</a></li>
    </ul> -->
</header>

<style>
    @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300&display=swap');

    * {
        margin: 0;
        padding: 0;
        box-sizing: border-box;
    }

    header {
        position: absolute;
        top: 0;
        left: 0;
        width: 100%;
        padding: 20px 100px;
        display: flex;
        align-items: center;
        justify-content: center;
        align-items: center;
        font-family: 'Poppins', sans-serif;
    }

    header a {
        text-decoration: none;
        color: black;
    }

    header .logo {
        position: relative;
        margin-left: 0%;
        max-width: 100px;
    }

    .name {
        margin-left: 35px;

        font-size: 1.1em;
        background-color: #f3ec78;
        background-image: linear-gradient(45deg, #eb8e59, #af4261);
        background-clip: text;
        background-size: 100%;
        -webkit-text-fill-color: transparent;
    }

    /* header ul {
        position: relative;
        display: flex;
    } */

    /* header ul li {
        list-style: none;
    } */

    /* header ul li a {
        display: inline-block;
        color: #000;
        font-weight: 400;
        margin-left: 40px;
        text-decoration: none;
    } */
</style>