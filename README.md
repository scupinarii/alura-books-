# alura-books-
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Aplicação Responsiva</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <h1>Meu Site Responsivo</h1>
    </header>
    <nav>
        <ul>
            <li><a href="#">Home</a></li>
            <li><a href="#">Sobre</a></li>
            <li><a href="#">Contato</a></li>
        </ul>
    </nav>
    <section class="content">
        <article>
            <h2>Título do Artigo</h2>
            <p>Conteúdo do artigo...</p>
        </article>
        <aside>
            <h3>Barra Lateral</h3>
            <p>Conteúdo adicional...</p>
        </aside>
    </section>
    <footer>
        <p>&copy; 2024 Meu Site Responsivo</p>
    </footer>
</body>
</html>
/* Estilo base para todos os dispositivos */
body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
}

header, nav, section, footer {
    padding: 1em;
}

header {
    background-color: #333;
    color: white;
    text-align: center;
}

nav ul {
    list-style: none;
    padding: 0;
    text-align: center;
    background-color: #444;
}

nav ul li {
    display: inline;
    margin: 0 15px;
}

nav ul li a {
    color: white;
    text-decoration: none;
}

.content {
    display: flex;
    flex-wrap: wrap;
}

article {
    flex: 2;
    padding: 10px;
}

aside {
    flex: 1;
    padding: 10px;
    background-color: #f4f4f4;
}

footer {
    background-color: #333;
    color: white;
    text-align: center;
}

/* Media query para dispositivos maiores */
@media (min-width: 768px) {
    .content {
        flex-direction: row;
    }

    nav ul {
        text-align: left;
    }

    nav ul li {
        display: inline;
    }
}
