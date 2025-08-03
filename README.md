# Lalo
Ventas
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
