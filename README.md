# 404notfound
 challenge


/** HTML CODE **/

<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>404 Not Found</title>
    <link rel="preload" href="css/normalize.css" as="styles">
    <link rel="stylesheet" href="css/normalize.css">
    <link rel="preload" href="css/styles.css" as="styles">
    <link rel="stylesheet" href="css/styles.css">
    <link href="https://fonts.googleapis.com/css2?family=Agdasima:wght@400;700&display=swap" rel="stylesheet">
</head>

<body>

    <header class="header contenedor">

        <h1 class="header__title">404 not found</h1>

    </header>

    <main class="contenedor">

        <div class="bloque">

            <div class="bloque__modificador">

                <h2 class="bloque__title">I have bad news for you</h2>

                <p class="bloque__text">The page you are looking for might be removed or is temporarily unavaible</p>

                <a class="boton bloque__boton" href="">back to homepage</a>

            </div>

            <img class="bloque__img" src="Scarecrow.png" alt="imagen error">

        </div>

    </main>

    <footer class="footer contenedor">

        <p class="footer__text">created by Shydou96 - devChallenges.io</p>
        
        <img class="dev_img" src="devchallenges.png" alt="dev img">

    </footer>

</body>

</html>


/** CSS CODE **/

:root {
    --fuentePrincipal: 'Agdasima', sans-serif;
    --black: #000;
    --white: #fff;
    --grey: #818181;
    --lightgrey: #bdb5b5;

}

html {
    box-sizing: border-box;
    font-size: 62.5%;
  }
  *, *:before, *:after {
    box-sizing: inherit;
  }

body {
    font-size: 1.6rem;
    font-family: var(--fuentePrincipal);
}

a {
    text-decoration: none;
}

img {
    width: 100%;
}

.contenedor {
    width: min(90%, 120rem);
    margin: 0 auto;
}

.boton {
    background-color: var(--black);
    color: var(--white);
    padding: 2rem 3rem;
    text-transform: uppercase;
    border-radius: .5rem;
    font-size: 1.8rem;
    display: inline-block;
}

/* Header */

.header {
    height: 15rem;
}

.header__title {
    text-transform: uppercase;
}

/* main */

.bloque {
    display: grid;
    grid-template-rows: repeat(2, auto);
}

@media (min-width: 768px) {
    .bloque {
        grid-template-columns: repeat(2, 1fr);
        margin-bottom: 10rem;
        gap: 10rem;
    }
}

.bloque__img {
    grid-row: 1 / 2;
    grid-column: 1 / 2;
}

.bloque__title {
    font-size: 7rem;
    margin-bottom: 0;
}

@media (min-width: 768px) {
    .bloque__title {
        font-size: 10rem;
    }
}

.bloque__text {
    font-size: 3rem;
    line-height: 1.5;
    color: var(--grey);
}


@media (min-width: 768px) {
    .bloque__img {
        height: 80%;
    }
}

.bloque__boton {
    margin: 2rem 0 10rem 0;
}

@media (min-width: 768px) {
    .bloque__boton {
        margin-top: 2rem;
    }
}


/* Footer */

.footer {
    display: flex;
    justify-content: center;
    gap: 3rem;
}

.footer__text {
    color: var(--lightgrey);
}

.dev_img {
    width: auto;
}