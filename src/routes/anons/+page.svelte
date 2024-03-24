<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Страница анонса</title>
    <style>
        body {
            background-color: #16202c; /* Темно-синий фон */
            color: #fff; /* Белый текст */
        }

        .announcement-container {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            margin-top: 50px;
            margin-left: 430px; /* Отступ сверху */
        }

        .announcement {
            margin-right: 40px;
            margin-bottom: 20px; /* Отступ между блоками */
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
            width: calc(50% - 40px);
            text-align: center;
            transition: transform 0.3s ease;
            background-color: #5e83d3;
        }

        .announcement img {
            width: 100%;
            height: auto;
            border-radius: 5px;
        }

        .announcement h3 {
            margin-top: 10px;
        }
    </style>
</head>
<body>
<div class="announcement-container">
    <div class="announcement" key="0">
        <img src="https://lightbox-prod.imgix.net/images/assets/100299171-7056477-Wrath_of_Man_2021_CC2.jpg" alt="Фильм 1">
        <h3>Гнев человеческий</h3>
        <p>Дата выхода: 10 сентября 2024</p>
    </div>
    <div class="announcement" key="1">
        <img src="https://vaiumdorama.com.br/wp-content/uploads/2020/02/snahp_image-2.jpg" alt="Фильм 2">
        <h3>Паразиты</h3>
        <p>Дата выхода: 15 сентября 2024</p>
    </div>
    <div class="announcement" key="2">
        <img src="https://pic.rutubelist.ru/video/f9/80/f9803ade017892c69824b5f160298ef0.jpg" alt="Фильм 3">
        <h3>Брат 2</h3>
        <p>Дата выхода: 20 сентября 2024</p>
    </div>
    <div class="announcement" key="3">
        <img src="https://pic.rutubelist.ru/video/f4/3e/f43e17ac9cce233b58f236b7d140a551.jpg"
             alt="Фильм 4">
        <h3>Линкольн для адвоката</h3>
        <p>Дата выхода: 25 сентября 2024</p>
    </div>
</div>
</body>
</html>
