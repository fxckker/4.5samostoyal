<div class="container">
    <h2>Наши модели</h2>
    <div class="model-row">
        <div class="model">
            <img src="https://zabavnikplus.ru/wp-content/uploads/b/c/3/bc32e97c0a66cbb4be71bb20841a5fe8.jpeg" alt="Model 1">
            <p>Дарья К</p>
        </div>
        <div class="model">
            <img src="https://74foto.ru/800/600/https/v.img.com.ua/b/1100x999999/b/3b/8093588692dfc6aa77cc3d1d4a7fa3bb.jpg" alt="Model 2">
            <p>Мария Л</p>
        </div>
    </div>
    <div class="model-row">
        <div class="model">
            <img src="https://mylitta.ru/uploads/posts/2013-11/1384095720_candice-swanepoel-04.jpg" alt="Model 3">
            <p>Полина В</p>
        </div>
        <div class="model">
            <img src="https://i.pinimg.com/originals/2a/8d/a6/2a8da660b9601fd12abf4bb39aaa6046.jpg" alt="Model 4">
            <p>Виктория М</p>
        </div>
    </div>
</div>

<style>
    .container {
    max-width: 1200px;
    margin: 0 auto;
    padding: 20px;
}

.model-row {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    margin-bottom: 20px;
    margin-left: 250px;
}

.model {
    flex-basis: calc(50% - 10px); /* Чтобы две модели помещались в строку */
    margin-bottom: 20px;
}

.model img {
    width: 100%;
    height: 700px; /* Фиксированная высота */
    object-fit: cover; /* Растягивает изображение, чтобы оно полностью заполнило контейнер */
}

.model p {
    margin-top: 5px;
    text-align: center;
}
</style>