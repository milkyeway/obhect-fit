<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Object-fit</title>
    <style>
        .box {
            width: 200px;
            height: 200px;
            overflow: hidden;
            margin: 30px;
            border: 3px solid rgb(254, 223, 225);
        }

        .box img {
            width: 100%;
            height: 100%;
            transition: .5s;
        }
        .box:hover img{
            transform: scale(1.5);
        }

        .fill {
            object-fit: fill;
        }

        .contain {
            object-fit: contain;
        }

        .cover {
            object-fit: cover;
            object-position: left top;
            /* 調整位置 預設為 center center */
        }

        .inherit {
            object-fit: inherit;
        }
        .none {
            object-fit: none;
            object-position: right top;
        }
    </style>

</head>

<body>
    <div class="box">
        <img class="fill" src="images/dr_strange.jpg" alt="">
    </div>
    <div class="box">
        <img class="contain" src="images/dr_strange.jpg" alt="">
    </div>
    <div class="box">
        <img class="cover" src="images/dr_strange.jpg" alt="">
    </div>
    <div class="box">
            <img class="inherit" src="images/dr_strange.jpg" alt="">
        </div>
        <div class="box">
                <img class="none" src="images/dr_strange.jpg" alt="">
            </div>
</body>

</html>
