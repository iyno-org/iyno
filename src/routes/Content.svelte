<script>
    import JournalImage from '$lib/images/Journal.jpg'
    import smallImg from '$lib/images/Journalresized.jpg'
</script>

<div class="content">
    <div class="textBox">
        <h2>Its not just a <span class="ttext">Neurosurgical</span> Organization.<br> Its an Organization for the <span class="ttext">Youth</span>.</h2>
        <p>This is some description about my organization. I would make this better. Lorem ipsum dolor sit amet consectetur adipisicing elit. Labore distinctio ratione enim commodi quam suscipit mollitia eligendi quaerat. Ad earum, quam cum quibusdam quidem libero provident fugiat ut nemo illo.</p>
    </div>
    <div class="imageBox">
        <img src="{JournalImage}" alt="Journal">
    </div>
</div>

<ul class="thumb">
    <li><img src="{smallImg}" alt="Journal"></li>
    <li><img src="{smallImg}" alt="Book"></li>
    <li><img src="{smallImg}" alt="AI"></li>
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