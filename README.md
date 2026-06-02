# -_mi_template_- :.
# Template Frontend Responsive:


```
## HTML + CSS + Visual Studio Code + Live Server
Este proyecto consiste en un **template frontend moderno tipo Landing Page** desarrollado con **HTML5 y CSS3** .

Incluye:
- Barra de navegación responsive
- Sección Hero (Inicio)
- Sección Servicios
- Sección Nosotros
- Formulario de Contacto
- Footer
- Diseño moderno y adaptable
- Compatible con Visual Studio Code + Live Server

---

# Estructura del Proyecto
```text
MiTemplate/
│
├── index.html
│
├── css/
│   └── estilos.css
│
└── img/
    └── logo.png
```

---

# Archivo: index.html

```html
<!DOCTYPE html>
<html lang="es">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mi Empresa</title>

    <link rel="stylesheet" href="css/estilos.css">
</head>

<body>

    <!-- NAVBAR -->

    <header>
        <nav class="navbar">

            <div class="logo">
                MiEmpresa
            </div>

            <ul class="menu">
                <li><a href="#inicio">Inicio</a></li>
                <li><a href="#servicios">Servicios</a></li>
                <li><a href="#nosotros">Nosotros</a></li>
                <li><a href="#contacto">Contacto</a></li>
            </ul>

        </nav>
    </header>

    <!-- HERO -->

    <section id="inicio" class="hero">

        <div class="hero-content">

            <h1>Bienvenido a Mi Empresa</h1>

            <p>
                Soluciones tecnológicas modernas para tu negocio.
            </p>

            <a href="#contacto" class="btn">
                Contáctanos
            </a>

        </div>

    </section>

    <!-- SERVICIOS -->

    <section id="servicios" class="servicios">

        <h2>Nuestros Servicios</h2>

        <div class="cards">

            <div class="card">
                <h3>Desarrollo Web</h3>
                <p>
                    Aplicaciones modernas con HTML, CSS,
                    JavaScript y tecnologías actuales.
                </p>
            </div>

            <div class="card">
                <h3>Base de Datos</h3>
                <p>
                    Integración con Oracle, MySQL y SQL Server.
                </p>
            </div>

            <div class="card">
                <h3>Soporte</h3>
                <p>
                    Mantenimiento y soporte para empresas.
                </p>
            </div>

        </div>

    </section>

    <!-- NOSOTROS -->

    <section id="nosotros" class="nosotros">

        <h2>Nosotros</h2>

        <p>
            Somos una empresa especializada en soluciones
            tecnológicas, desarrollo de software y
            transformación digital.
        </p>

    </section>

    <!-- FORMULARIO -->

    <section id="contacto" class="contacto">

        <h2>Formulario de Contacto</h2>

        <form>

            <input
                type="text"
                placeholder="Nombre Completo"
                required>

            <input
                type="email"
                placeholder="Correo Electrónico"
                required>

            <input
                type="text"
                placeholder="Asunto"
                required>

            <textarea
                rows="6"
                placeholder="Escribe tu mensaje..."
                required></textarea>

            <button type="submit">
                Enviar
            </button>

        </form>

    </section>

    <!-- FOOTER -->

    <footer>

        <p>
            © 2026 Mi Empresa - Todos los derechos reservados
        </p>

    </footer>

</body>
</html>
```

---

# Archivo: css/estilos.css

```css
/* RESET */

*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    font-family:Arial, Helvetica, sans-serif;
}

/* BODY */

body{
    background:#f4f6f9;
    color:#333;
}

/* NAVBAR */

.navbar{
    display:flex;
    justify-content:space-between;
    align-items:center;
    padding:20px 10%;
    background:#1e293b;
}

.logo{
    color:white;
    font-size:28px;
    font-weight:bold;
}

.menu{
    display:flex;
    list-style:none;
    gap:25px;
}

.menu a{
    text-decoration:none;
    color:white;
    transition:0.3s;
}

.menu a:hover{
    color:#38bdf8;
}

/* HERO */

.hero{
    height:90vh;
    display:flex;
    justify-content:center;
    align-items:center;
    text-align:center;

    background:linear-gradient(
        rgba(0,0,0,0.6),
        rgba(0,0,0,0.6)
    ),
    url("https://images.unsplash.com/photo-1498050108023-c5249f4df085");

    background-size:cover;
    background-position:center;
}

.hero-content{
    color:white;
}

.hero h1{
    font-size:60px;
    margin-bottom:20px;
}

.hero p{
    font-size:22px;
    margin-bottom:30px;
}

.btn{
    display:inline-block;
    padding:15px 35px;
    background:#38bdf8;
    color:white;
    text-decoration:none;
    border-radius:8px;
}

.btn:hover{
    background:#0ea5e9;
}

/* SERVICIOS */

.servicios{
    padding:80px 10%;
    text-align:center;
}

.servicios h2{
    margin-bottom:50px;
    font-size:40px;
}

.cards{
    display:flex;
    gap:30px;
    flex-wrap:wrap;
    justify-content:center;
}

.card{
    background:white;
    width:300px;
    padding:30px;
    border-radius:10px;
    box-shadow:0 5px 15px rgba(0,0,0,.1);
}

.card h3{
    margin-bottom:15px;
}

/* NOSOTROS */

.nosotros{
    padding:80px 10%;
    text-align:center;
    background:white;
}

.nosotros h2{
    margin-bottom:20px;
    font-size:40px;
}

.nosotros p{
    max-width:800px;
    margin:auto;
    line-height:1.8;
}

/* CONTACTO */

.contacto{
    padding:80px 10%;
}

.contacto h2{
    text-align:center;
    margin-bottom:40px;
    font-size:40px;
}

form{
    max-width:700px;
    margin:auto;

    display:flex;
    flex-direction:column;
    gap:15px;
}

input,
textarea{
    padding:15px;
    border:1px solid #ccc;
    border-radius:8px;
}

button{
    padding:15px;
    border:none;
    background:#1e293b;
    color:white;
    cursor:pointer;
    border-radius:8px;
    font-size:18px;
}

button:hover{
    background:#334155;
}

/* FOOTER */

footer{
    background:#1e293b;
    color:white;
    text-align:center;
    padding:25px;
}

/* RESPONSIVE */

@media(max-width:768px){

    .navbar{
        flex-direction:column;
        gap:15px;
    }

    .menu{
        flex-direction:column;
        text-align:center;
    }

    .hero h1{
        font-size:40px;
    }

    .hero p{
        font-size:18px;
    }

}
```

---

```

# Ejecución con Live Server

## Paso 1

Instalar la extensión **Live Server** en Visual Studio Code.

## Paso 2

Abrir la carpeta del proyecto:

```text
MiTemplate

```

```
## Paso 3

Abrir el archivo:

```text
index.html
```

```
## Paso 4

Clic derecho sobre el archivo y seleccionar:

```text
Open with Live Server
```

---

```
# Resultado

El navegador abrirá automáticamente una URL similar a:

```text
http://127.0.0.1:5500/index.html
```

---

```
# Características del Template

- Diseño moderno tipo Landing Page
- Navegación por anclas
- Responsive Design
- Hero con imagen de fondo
- Tarjetas de servicios
- Sección institucional
- Formulario de contacto
- Footer corporativo
- Fácil personalización

---

# Posibles Mejoras Futuras

Este template puede utilizarse posteriormente para conectar un backend desarrollado en:

- Java Spring Boot
- PHP
- Node.js
- ASP.NET
- Python Django
- Python Flask

También puede integrarse con bases de datos como:

- Oracle 19c
- MySQL
- PostgreSQL
- SQL Server

---

# Conclusión

Este proyecto proporciona una base sólida para desarrollar sitios web corporativos, landing pages y sistemas empresariales. Su estructura sencilla facilita la integración futura con APIs, servicios web y bases de datos empresariales como Oracle Database 19c .
:. . / .
