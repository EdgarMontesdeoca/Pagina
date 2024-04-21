<!DOCTYPE html>
<html lang="es">
<head>
    <title>Ejemplo de maquetación</title>
    <link rel="stylesheet" href="Codigoweb.css">
</head>
<body>
    <header>
        <div class="container">
            <p class="logo">Curso IBM</p>
            <nav>
                <a href="#somos-Bejob">Quienes Somos</a>
                <a href="#nuestros-programas">Nuestros Programas</a>
                <a href="#caracteristicas">Características</a>
            </nav>
        </div>
    </header>

    <section id="hero">
        <h1>Aprende a Programar <br>con los Mejores</h1>
        <button>Ingresar!</button>
    </section>

    <section id="somos-Bejob">
        <div class="container">
            <div class="img-container"></div>
            <div class="texto">
                <h2>Somos <span class="color-acento">Woman4IT</span></h2>
                <p>(IBM) es una compañía estadounidense privada que provee soluciones de hardware, entre los que se incluyen computadoras portátiles y de escritorio,
y sistemas de mainframes, servidores y almacenamiento, así como software, servicios financieros y una amplia gama de servicios de tecnología de información.</p>
            </div>
        </div>
    </section>

    <section id="nuestros-programas">
        <div class="container">
            <h2>Nuestros Programas</h2>
            <div class="programas">
                <div class="cursos">
                    <h3>Programador Front-end</h3>
                    <p>Un desarrollador front-end es el programador que se encarga de 
que una web sea atractiva para el usuario y, al mismo tiempo, funcione correctamente. 
Su alta demanda hace que la de front-end developer se coloque en lo alto del ranking 
de una de las profesiones más cotizadas.</p>
                    <button>+ Info</button>
                </div>
                <div class="cursos">
                    <h3>Programador Full-Stack</h3>
                    <p>¿Qué es un Desarrollador full stack? El desarrollador Full Stack se encarga de crear 
y mantener las partes de front y back end de una aplicación web, con polivalencia para el conocimiento de 
lenguajes de programación y sistemas operativos. Su objetivo es coordinar los procesos de desarrollo 
y producción de software.</p>
                    <button>+ Info</button>
                </div>
                <div class="cursos">
                    <h3>Programador Python</h3>
                    <p>Desde el desarrollo de aplicaciones web hasta el análisis de grandes volúmenes de datos,
lo que hace un programador Python abarca una amplia gama de desafíos y contribuye al éxito de todo tipo de proyectos.</p>
                    <button>+ Info</button>
                </div>
            </div>
        </div>
    </section>

    <section id="caracteristicas">
        <div class="container">
            <ul>
                <li>✔️ 100% online</li>
                <li>✔️ Flexibilidad de horarios</li>
                <li>✔️ Soporte 1:1</li>
                <li>✔️ Asistencia financiera</li>
            </ul>
        </div>
    </section>

    <section id="final">
        <h2>Listo para programar?</h2>
        <button>Ingresar!</button>
    </section>

    <footer>
        <div class="container">
            <p>&copy; Curso 2024
                By edgar
            </p>
        </div>
    </footer>
</body>
</html>

/* Establece que al agregar margin o padding a los elementos, no crezcan más allá del borde de su contenedor */
* {
    box-sizing: border-box;
}

/* Configuración general */
html {
    scroll-behavior: smooth;
}

body {
    /* Fuente predeterminada */
    font-family: 'Roboto', sans-serif;
    /* Elimina el margen predeterminado del body */
    margin: 0;
}

/* Cambios en el tamaño de fuente */
h1 { font-size: 3.5em; }
h2 { font-size: 2.7em; }
h3 { font-size: 2em; }
p { font-size: 1.25em; }
ul { list-style: none; }
li { font-size: 1.25em; }

button {
    font-size: 1.25em;
    font-weight: bold;
    padding: 10px 30px;
    border-radius: 5px;
    border: 2px solid rgba(0, 0, 0, 0.3);
    box-shadow: 2px 2px 10px rgba(0, 0, 0, 0.5);
    color: white;
    background-color: blueviolet;
}

button:hover {
    background-color: rgb(101, 33, 165);
}

.container {
    max-width: 1400px;
    margin: auto;
}

.color-acento {
    color: blueviolet;
}

/* Estilos para la barra de navegación */
header {
    background-color: rgb(245, 245, 245);
}

header .logo {
    margin: 0;
    padding: 25px 30px;
    font-weight: bold;
    color: blueviolet;
    font-size: 1.6em;
}

header .container {
    display: flex;
    flex-direction: column;
    align-items: center;
}

header nav {
    display: flex;
    flex-direction: column;
    text-align: center;
    padding-bottom: 25px;
}

header a {
    padding: 5px 12px;
    text-decoration: none;
    font-weight: bold;
    color: black;
}

header a:hover {
    color: blueviolet;
}

/* Estilos para la sección del héroe */
#hero {
    display: flex;
    align-items: center;
    justify-content: center;
    text-align: center;
    flex-direction: column;
    height: 90vh;
    background-image: linear-gradient(0deg, rgba(0,0,0,0.5), rgba(0,0,0,0.5)), url(media/hero.jpg);
    background-repeat: no-repeat;
    background-size: cover;
    background-position: center center;
}

#hero h1 {
    color: white;
}

#hero button {
    font-size: 1.75em;
}

/* Estilos para la sección "Somos Woman4IT" */
#somos-Bejob .container {
    text-align: center;
    padding: 200px 12px;
}

/* Estilos para la sección de nuestros programas */
#nuestros-programas {
    background-color: rgb(30, 30, 30);
    color: white;
    text-align: center;
}

#nuestros-programas .container {
    padding: 150px 12px;
}

#nuestros-programas h2 {
    margin-top: 0;
    font-size: 3.2em;
}

#nuestros-programas p {}

#nuestros-programas .cursos {
    background-position: center center;
    background-size: cover;
    padding: 50px 0px;
    margin: 30px;
    border-radius: 15px;
}

/* Estilos para las imágenes de los cursos */
.cursos:first-child {
    background-image: linear-gradient(0deg, rgba(0,0,0,0.6), rgba(0,0,0,0.6)), url(media/front-end.jpg);
}

.cursos:nth-child(2) {
    background-image: linear-gradient(0deg, rgba(0,0,0,0.6), rgba(0,0,0,0.6)), url(media/full-stack.jpg);
}

.cursos:nth-child(3) {
    background-image: linear-gradient(0deg, rgba(0,0,0,0.6), rgba(0,0,0,0.6)), url(media/python.jpg);
}

/* Estilos para la sección de características */
#caracteristicas .container {
    text-align: center;
    padding: 250px 12px;
}

#caracteristicas li {
    margin: 16px 0px;
    font-weight: bold;
}

/* Estilos para la sección final */
#final {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    text-align: center;
    background-color: rgb(30, 30, 30);
    color: white;
    height: 80vh;
}

#final h2 {
    font-size: 9vw;
}

#final button {
    font-size: 5vw;
}

/* Estilos para el pie de página */
footer {
    background-color: rgb(230, 230, 230);
}

footer p {
    margin: 0;
    padding: 12px;
    color: rgb(100, 100, 100);
}

footer .container {
    height: 150px;
    display: flex;
    justify-content: center;
    align-items: flex-end;
}

/* Media queries */
@media (min-width: 850px) {
    header {
        position: fixed;
        width: 100%;
    }

    header .container {
        flex-direction: row;
        justify-content: space-between;
    }

    header nav {
        flex-direction: row;
        padding-bottom: 0;
        padding-right: 30px;
    }

    #hero h1 {
        font-size: 5em;
    }

    #somos-Bejob .container {
        display: flex;
        justify-content: space-evenly;
    }

    #somos-Bejob .texto {
        width: 50%;
        max-width: 600px;
        text-align: initial;
        padding-left: 30px;
        display: flex;
        flex-direction: column;
        justify-content: center;
    }

    #nuestros-programas .programas {
        display: flex;
        justify-content: center;
    }

    #nuestros-programas p {
        display: block;
        margin-bottom: 30px;
    }

    #nuestros-programas h2 {
        font-size: 4em;
    }

    #nuestros-programas h3 {
        margin-top: 0;
    }

    #nuestros-programas .cursos {
        padding: 50px;
    }

    footer .container {
        justify-content: flex-end;
    }

    #final h2 {
        font-size: 5em;
    }

    #final button {
        font-size: 2em;
    }
}

@media (min-width: 1200px) {
    #caracteristicas {
        background-position-x: calc(100vw - 800px);
    }
}

