<!DOCTYPE html>
<svelte:head>
<title>Maxim Cinema</title>
</svelte:head>

<body>
    <div class ="container">
        <div class="info">
            <div class = "animate-background">
                <div class="container info-container">
                    <div class="info-text">
                        <h1>
                            <p class="animate-text-1">Maxim Cinema</p>
                        </h1>
                    </div>
                    <h2 class="subtitle">
                        Вас приветствует одна из крупнейших кинопрокатных сетей. Наши кинотеатры соответствуют мировым стандартам качества кинопоказа. Современные видео- и аудио- системы, а также комфортные кресла, позволяют зрителю полностью окунуться в атмосферу кино и получить максимум удовольствия от просмотра.
                    </h2>
                    <div style="color:black" class="scroll-button animate-scroll" tabindex="0">
                        <a href="/catalog">Расписание сеансов</a>
                    </div>
                </div>
            </div>
        </div>
    </div> 
    
    <style>
    
/* Общие стили */
body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    background-image: url('https://files.vgtimes.ru/posts/2020-06/1593195992_755852177483339.jpg');
    background-size: cover;
    background-position: center;
    background-repeat: no-repeat;
}

.blur-background {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    filter: blur(5px);
    z-index: -1; /* Перемещаем фон за блок .info */
}

.container {
    max-width: 1200px;
    margin: 0 auto;
    padding: 20px;
    position: relative; /* Добавляем позиционирование */
    z-index: 1; /* Помещаем блок .info поверх фона */
}

/* Стили для информации о кинотеатре */
.info {
    background-color: #003366;
    border-radius: 10px;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
    padding: 20px;
    margin-top: 50px;
}

.info-container {
    display: flex;
    flex-direction: column;
    align-items: center;
}

.info-text {
    text-align: center;
    margin-bottom: 20px;
}

h1 {
    margin: 0;
    font-size: 50px;
    color: #fff;
}

.subtitle {
    font-size: 28px;
    color: #fff;
    text-align: center;
    max-width: 800px;
}

.scroll-button {
    text-align: center;
    margin-top: 20px;
}

.scroll-button a {
    display: inline-block;
    background-color: #87cefa;
    color: #000000;
    padding: 10px 20px;
    border-radius: 5px;
    text-decoration: none;
    transition: background-color 0.3s ease;
}

.scroll-button a:hover {
    background-color: #0056b3;
}

/* Анимации */
@keyframes fadeIn {
    from {
        opacity: 0;
    }
    to {
        opacity: 1;
    }
}

.animate-background {
    animation: fadeIn 1s ease forwards;
}

.animate-text-1 {
    animation: fadeIn 1s ease forwards;
    animation-delay: 0.5s;
}

.animate-scroll {
    animation: fadeIn 1s ease forwards;
    animation-delay: 1s;
}


    </style>
</body>