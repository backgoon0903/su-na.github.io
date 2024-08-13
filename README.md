
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Title</title>
</head>
<body>

<style>
    .box{
        border: 1px solid black;
        box-sizing: border-box;
        height: 50vh;
        width: 50vw;
        display: none;

    }
    .b1{
        background-color: pink;
    }
    .b2{
        background-color: skyblue;
    }
    .show{
        display: block;
    }

</style>


<div class="cotainer">
    <div class="menu">
        <ul>
            <button><li onclick="showMenu('b1')">수진</li></button>
            <button><li onclick="showMenu('b2')">나경</li></button>
        </ul>
    </div>
    <div class="box b1 show">
        <h1>언제와</h1>
    </div>
    <div class="box b2">
        <h1>뭐하니</h1>
    </div>

</div>


<ul class="menuUL">

</ul>

<script>
    const b1 = document.querySelector('.b1')
    const b2 = document.querySelector('.b2')


    function showMenu(target){
        document.querySelectorAll('.box').forEach(box =>{
            box.classList.remove('show')
        })
        document.querySelector(`.${target}`).classList.add('show')
    }



</script>

</body>
</html>
