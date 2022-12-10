<script>
    import { fly } from 'svelte/transition';
    import JournalImage from '$lib/images/Journal.jpg'
    import smallImg from '$lib/images/Journalresized.jpg'
    let number = 0;

        let text1i = "Its not just a"
        let span1 = "Neurosurgical"
        let text1f = "Organization"
        let text2i = "This is an Organization for"
        let span2 = "Youth."

    function changeText1(){
        number += 1
        text1i = "Read the"
        span1 = "Journal"
        text1f = "by the IYNA"
        text2i = "A Journal for"
        span2 = "Young and Aspiring Neurosurgeons."
        visible = true
    }

    function changeText2(){
        number += 1
        text1i = "Read the"
        span1 = "Book"
        text1f = "by the IYNA"
        text2i = "The book that tries to make"
        span2 = "Neurosurgery Easy!"
    }

    function changeText3(){
        number += 1
        text1i = "Discover our work on"
        span1 = "AI"
        text1f = "that helps you learn"
        text2i = "Ai should help us become better. Not"
        span2 = "Replace us!"
    }
    
</script>



<div class="content">
    <div class="textBox">
        {#key number}
        <h2 class="header">{text1i} <span>{span1}</span> {text1f}.<br>{text2i} <span>{span2}</span></h2>
        {/key}

        <p>This is some description about my organization. I would make this better. Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
    </div>
    <div class="imageBox">
        <img src="{JournalImage}" alt="Journal">
    </div>
</div>

<ul class="thumb">
    <li><img src="{smallImg}" alt="Journal" on:click={changeText1}></li>
    <li><img src="{smallImg}" alt="Book" on:click={changeText2}></li>
    <li><img src="{smallImg}" alt="AI" on:click={changeText3}></li>
</ul>

<style>
    @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300&display=swap');

    * {
        margin: 0;
        padding: 0;
        box-sizing: border-box;
    }

    .content {
        font-family: 'Poppins', sans-serif;
        position: relative;
        width: 100%;
        display: flex;
        justify-content: space-between;
        align-items: center;
    }
    
    .content .textBox {
        position: relative;
        min-height: 50vh;
        max-width: 1000px;
        margin-left: 20px;
        padding: 80px;
        /* blur */
        background: rgba(255, 255, 255, 0.2);
        border-radius: 16px;
        box-shadow: 0 4px 30px rgba(0, 0, 0, 0.1);
        backdrop-filter: blur(5px);
        -webkit-backdrop-filter: blur(5px);
        border: 1px solid rgba(255, 255, 255, 0.3);
    }

    .content .textBox h2 {
        font-size: 2.5em;
        line-height: 1.4em;
        animation: fadein 2s;
    }
    @keyframes fadein {
        from { opacity: 0; }
        to   { opacity: 1; }
    }
    @keyframes fadein {
    from { opacity: 0; }
    to   { opacity: 1; }
    }

    .content .textBox h2 span {
        font-size: 1.1em;
        background-color: #f3ec78;
        background-image: linear-gradient(45deg, #eb8e59, #af4261);
        background-clip: text;
        background-size: 100%;
        -webkit-text-fill-color: transparent;
    }

    .content .textBox p {
        font-size: 20px;
        margin-top: 20px;
    }

    .content .imageBox {
        width: 600px;
        display: flex;
        justify-content: flex-end;
        padding-right: 50px;
        margin-top: 50px;
    }

    .content .imageBox img {
        max-width: 450px;
    }

    .thumb {
        position: absolute;
        left: 50%;
        bottom: 50px;
        transform: translateX(-50%);
        display: flex;
    }
    
    .thumb li {
        list-style: none;
        display: inline-block;
        margin: 0px 20px;
        cursor: pointer;
        transition: 0.25s;
    }

    .thumb li:hover {
        transform: translateY(-15px);
    }
</style>