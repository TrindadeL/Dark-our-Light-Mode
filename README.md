# Dark-our-Light-Mode
Modo escuro ou claro
function changeMode () {
    changeClasses ();
    changeText();
}

function changeClasses() {
    button.classList.toggle(darkModeClass);
    h1.classList.toggle(darkModeClass);
    body.classList.toggle(darkModeClass);
    footer.classList.toggle(darkModeClass);
}

function changeText() {
    const lightMode = 'Light Mode';
    const darkMode = 'Dark Mode';
}

    if (body.classList.contains(darkModeClass)) {
        button.innerHTML = lightMode;
        h1.innerHTML = darkMode + ' ON';
        return;
    }

    button.innerHTML = darkMode; {
    h1.innerHTML = lightMode + ' ON';
}

const darkModeClass = 'dark-mode';
const button = document.getElementById ('mode-selector');
const h1 = document.getElementById('page-title');
const body = document.getElementsByTagName ('body')[0];
const footer = document.getElementsByTagName('footer')[0];

button.addEventListener('clicl', changeMode);




<!DOCTYPE html>
<html lang="eng">
    <head>
        <meta charset=""UTF-8" />
        <meta http-equi v="X-UA-Compatible" content="IE=edge" />
        <meta name="viewport" content="width=device-width, initial-scale=1.0" />
        <link rel="stylesheet" href="assets/css/styles.css" />
        <title> Dark mode and Light Mode</title>
    </head>
    <body>
        <main>
            <h1 id="page-title">Light Mode ON</h1>
            <button aria-label="selecionar-modo" id="mode-selector">Dark Mode</button>
        </main>

        <footer>Basecamp Javascript @ Digital Innovation One</footer>
        <script src="assets/js/scripts.js"></script>
    </body>
</html>
