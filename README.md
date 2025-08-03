# Lalo
Ventas
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mi Negocio</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <header>
        <h1>Bienvenidos a Mi Negocio</h1>
        <p>Descubre nuestros increíbles productos.</p>
    </header>

    <main>
        <section id="galeria">
            <h2>Nuestros Productos</h2>
            <div class="galeria-fotos">
                <img src="https://via.placeholder.com/150" alt="Producto 1">
                <img src="https://via.placeholder.com/150" alt="Producto 2">
                <img src="https://via.placeholder.com/150" alt="Producto 3">
                </div>
        </section>

        <section id="precios">
            <h2>Lista de Precios</h2>
            <ul class="lista-precios">
                <li>
                    <span>Producto A</span>
                    <span>$10.00</span>
                </li>
                <li>
                    <span>Producto B</span>
                    <span>$25.50</span>
                </li>
                <li>
                    <span>Producto C</span>
                    <span>$5.99</span>
                </li>
                </ul>
        </section>

        <section id="contacto">
            <h2>Contacto</h2>
            <form id="formulario-contacto">
                <label for="nombre">Nombre:</label>
                <input type="text" id="nombre" name="nombre" required>

                <label for="email">Email:</label>
                <input type="email" id="email" name="email" required>

                <label for="mensaje">Mensaje:</label>
                <textarea id="mensaje" name="mensaje" rows="4" required></textarea>

                <button type="submit">Enviar Mensaje</button>
            </form>
        </section>
    </main>

    <footer>
        <p>&copy; 2024 Mi Negocio. Todos los derechos reservados.</p>
    </footer>

    <script src="script.js"></script>
</body>
</html>

body {
    font-family: sans-serif;
    margin: 0;
    padding: 0;
    background-color: #f4f4f4;
    color: #333;
}

header {
    background-color: #007BFF;
    color: white;
    padding: 1em 0;
    text-align: center;
}

main {
    padding: 20px;
}

section {
    background-color: white;
    margin-bottom: 20px;
    padding: 20px;
    border-radius: 8px;
    box-shadow: 0 2px 4px rgba(0,0,0,0.1);
}

/* Estilos de la Galería */
.galeria-fotos {
    display: flex;
    flex-wrap: wrap;
    gap: 10px;
    justify-content: center;
}

.galeria-fotos img {
    width: 100px;
    height: 100px;
    object-fit: cover;
    border-radius: 4px;
}

/* Estilos de la Lista de Precios */
.lista-precios {
    list-style: none;
    padding: 0;
}

.lista-precios li {
    display: flex;
    justify-content: space-between;
    padding: 10px 0;
    border-bottom: 1px solid #eee;
}

/* Estilos del Formulario */
#formulario-contacto label {
    display: block;
    margin-top: 10px;
}

#formulario-contacto input,
#formulario-contacto textarea {
    width: 100%;
    padding: 8px;
    margin-top: 5px;
    border: 1px solid #ccc;
    border-radius: 4px;
}

#formulario-contacto button {
    background-color: #007BFF;
    color: white;
    padding: 10px 15px;
    border: none;
    border-radius: 4px;
    cursor: pointer;
    margin-top: 10px;
}

#formulario-contacto button:hover {
    background-color: #0056b3;
}

footer {
    text-align: center;
    padding: 10px 0;
    background-color: #333;
    color: white;
}
document.addEventListener('DOMContentLoaded', () => {
    const formulario = document.getElementById('formulario-contacto');

    formulario.addEventListener('submit', (evento) => {
        evento.preventDefault(); // Evita que la página se recargue

        // Puedes recoger los datos del formulario si lo necesitas
        const nombre = document.getElementById('nombre').value;
        const email = document.getElementById('email').value;
        const mensaje = document.getElementById('mensaje').value;

        // Aquí podrías enviar los datos a un servidor, pero por ahora solo mostraremos un mensaje
        alert(`¡Gracias por tu mensaje, ${nombre}! Nos pondremos en contacto contigo pronto.`);
        
        formulario.reset(); // Limpia los campos del formulario
    });
});
