<script>
    import logo from "$lib/images/brain.png"
</script>

<header>
    <a href="/" class="logo"><img src="{logo}" alt="logo"></a>
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
        justify-content: space-between;
        align-items: center;
        font-family: 'Poppins', sans-serif;
    }

    header .logo {
        position: relative;
        margin-left: 50%;
        max-width: 100px;
    }

    header ul {
        position: relative;
        display: flex;
    }
    header ul li {
        list-style: none;
    }

    header ul li a {
        display: inline-block;
        color: #000;
        font-weight: 400;
        margin-left: 40px;
        text-decoration: none;
    }
</style>