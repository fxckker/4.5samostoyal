<nav>
    <div class = "nav-container">
        <a href="/" class ="nav-logo" title="Back to Homepages">Maxim Cinema</a>
        <div class="nav-links">
            {#each nav as link}
                <a href={link.href} class="link">{link.title}</a>
            {/each}
        </div>
    </div>
</nav>

<div class="container">
    <!--Pages will be injected below-->
    <slot></slot>
</div>

<script>
    const nav = [
        {
            title: "Каталог",
            href: "/catalog"
        },
        {
            title: "Анонс",
            href: "/anons"
        },
        {
            title: "Контакты",
            href: "/contact"
        }
    ]
</script>

<style>
    .container{
        max-width: 1400px;
        margin: 50 px auto;
    }
nav {
    background-color: #5e83d3;
    padding: 10px 0;
    width: 100%;
    margin-left: calc(-50vw + 50%);
    margin-right: calc(-50vw + 50%);
    position: relative;
}

.nav-container {
    display: flex;
    justify-content: space-between;
    align-items: center;
    max-width: 1200px;
    margin: 0 auto;
    padding: 0 20px;
}

.nav-logo {
    color: #fff;
    text-decoration: none;
    font-size: 24px;
    font-weight: bold;
    margin-right: 100px; /* Выравнивание текста к левому краю */
}

.nav-links {
    display: flex;
}

.link {
    color: #fff;
    text-decoration: none;
    margin-left: 20px;
}

.link:hover {
    text-decoration: underline;
}
</style>