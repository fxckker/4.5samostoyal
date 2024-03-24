<!DOCTYPE html>
<body>
    <div class="movie-container" id="app">
        <div class="movie" key="0">
            <img src="https://wallpapercave.com/wp/wp4549292.jpg"
                 alt="Фильм 1">
            <h3>Project X</h3>
            <label for="time-movie1">Выберите время сеанса:</label>
            <select id="time-movie1">
                <option value="10:00">10:00</option>
                <option value="13:00">13:00</option>
                <option value="16:00">16:00</option>
            </select>
            <br>
            <label for="tickets-movie1">Выберите количество билетов:</label>
        <select id="tickets-movie1">
            <option value="1">1</option>
                <option value="2">2</option>
                <option value="3">3</option>
                <option value="4">4</option>
                <option value="5">5</option>
            <!-- Добавьте другие варианты, если необходимо -->
        </select>
            <button class="book-button" onclick="bookTickets(0)">Забронировать</button>
        </div>
        <div class="movie" key="1">
            <img src="https://images6.alphacoders.com/126/1269171.jpg"
                 alt="Фильм 2">
            <h3>Fight Club</h3>
            <label for="time-movie2">Выберите время сеанса:</label>
            <select id="time-movie2">
                <option value="11:00">11:00</option>
                <option value="14:00">14:00</option>
                <option value="17:00">17:00</option>
            </select>
            <br>
            <label for="tickets-movie2">Выберите количество билетов:</label>
            <select id="tickets-movie2">
                <option value="1">1</option>
                <option value="2">2</option>
                <option value="3">3</option>
                <option value="4">4</option>
                <option value="5">5</option>
                <!-- Добавьте другие варианты, если необходимо -->
            </select>
            <button class="book-button" onclick="bookTickets(1)">Забронировать</button>
        </div>
        <div class="movie" key="2">
            <img src="https://i.playground.ru/p/vwTxY0WaUuHUvFAaak_mgA.png"
                 alt="Фильм 3">
            <h3>Брат</h3>
            <label for="time-movie3">Выберите время сеанса:</label>
            <select id="time-movie3">
                <option value="12:00">12:00</option>
                <option value="15:00">15:00</option>
                <option value="18:00">18:00</option>
            </select>
            <br>
            <label for="tickets-movie3">Выберите количество билетов:</label>
            <select id="tickets-movie3">
                <option value="1">1</option>
                <option value="2">2</option>
                <option value="3">3</option>
                <option value="4">4</option>
                <option value="5">5</option>
                <!-- Добавьте другие варианты, если необходимо -->
            </select>
            <button class="book-button" onclick="bookTickets(2)">Забронировать</button>
        </div>
        <div class="movie" key="3">
            <img src="https://canaltrece.com.co/uploads/newsarticle/436a7c75ca744dfe8f5461e5763fbdfe/the_broken_and_the_bad-min-min_1.jpg"
                 alt="Фильм 4">
            <h3>Во все тяжкие</h3>
            <label for="time-movie4">Выберите время сеанса:</label>
            <select id="time-movie4">
                <option value="13:00">13:00</option>
                <option value="16:00">16:00</option>
                <option value="19:00">19:00</option>
            </select>
            <br>
            <label for="tickets-movie4">Выберите количество билетов:</label>
            <select id="tickets-movie4">
                <option value="1">1</option>
                <option value="2">2</option>
                <option value="3">3</option>
                <option value="4">4</option>
                <option value="5">5</option>
                <!-- Добавьте другие варианты, если необходимо -->
            </select>
            <button class="book-button" onclick="bookTickets(3)">Забронировать</button>
        </div>
    </div>
    
    <script>
        function bookTickets(index) {
            const movieTitle = document.querySelectorAll('.movie h3')[index].innerText;
            const timeSelect = document.getElementById(`time-movie${index + 1}`);
            const selectedTime = timeSelect.options[timeSelect.selectedIndex].value;
            const ticketsInput = document.getElementById(`tickets-movie${index + 1}`);
            const totalTickets = parseInt(ticketsInput.value);
            const totalPrice = totalTickets * 10;
            alert(`Вы успешно купили ${totalTickets} билет(ов) на "${movieTitle}" на время ${selectedTime} за цену ${totalPrice}$`);
        }
    </script>
   <style>
    body {
    background-color: #16202c; /* Темно-синий фон */
    color: #fff; /* Белый текст */
}
    .movie-container {
        display: flex;
        flex-wrap: wrap;
        margin-left: 400px;
        margin-top: 30px;
    }
    .movie {
    background-color: #5e83d3; /* Голубой фон */
    margin-right: 40px;
    margin-bottom: 20px;
    padding: 20px;
    border-radius: 10px;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
    width: calc(50% - 40px);
    text-align: center;
    transition: transform 0.3s ease;
}
        .movie:hover {
        transform: translateY(-5px);
    }
    .movie img {
        width: 100%;
        height: auto; /* Автоматическое подстраивание высоты изображений */
        border-radius: 5px;
    }
    .book-button {
    display: block;
    margin-top: 10px;
    padding: 10px 20px;
    border: none;
    border-radius: 5px;
    background-color: #0056b3; /* Темно-голубая кнопка */
    color: #fff;
    font-size: 16px;
    cursor: pointer;
    transition: background-color 0.3s ease;
    margin-left: 135px
}
.book-button:hover {
    background-color: #004080; /* Уменьшенная насыщенность для кнопки при наведении */
}
</style>
  </body>
