<svelte:head>
<title>Model Agency MAXIM</title>
</svelte:head>

<div class ="container">
    <div class="info">
        <div class = "animate-background">
            <div class="container info-container">
                <div class="info-text">
                    <h1>
                        <p class="animate-text-1">Model Agency</p>
                        <p class="text-2">Модельное агентство MAXIM</p>
                    </h1>
                </div>
                <h2 class="subtitle">
                    Вы когда-нибудь задумывались о том, сколько дорог и перекрёстков предоставляет нам жизнь? Берите то, что даёт вам судьба! Возможно, впереди то самое будущее, о котором вы мечтаете, нужно просто открыться ему. Очень трудно вернуть упущенное время, а порой и невозможно. Позвольте чудесам случиться!Приходите в моё агентство!
                </h2>
                <div style="color:black" class="scroll-button animate-scroll" tabindex="0">
                    <a href="/models">Модели →</a>
                </div>
            </div>
        </div>
    </div>
</div>

<div class="background-div"></div>

<style>
    .info {
        text-align: center;
        position: relative;
    }

    .info-container {
        height: 100%;
        display: flex;
        flex-direction: column;
        justify-content: center;
        text-align: left;
        align-items: start;
    }

    .container {
        max-width: 1400px;
        margin: 190px 0 0 2.5rem;
    }

    .info h1 {
        font-size: 4rem;
        margin: 0;
    }

    .info h1 p {
        position: relative;
        font: inherit;
        margin: 0;
        text-align: left;
        line-height: 130%;
        width: fit-content;
        font-weight: 800;
        letter-spacing: -0.03em;
    }

    .info h2 {
        max-width: 65ch;
        font-weight: 200;
        margin-top: 0.50rem;
    }
    
    .background-div {
        background-color: #bcb4db;
        width: 200%;
        height: 56vh;
        margin: -205px auto;
    }
    .info .info-text{
        position: relative;
    }

    .scroll-button {
    display: inline-block;
    background-color: #8375ac;
    color: #fff;
    padding: 10px 20px;
    border-radius: 5px;
    text-decoration: none;
    transition: background-color 0.3s ease;
}
</style>