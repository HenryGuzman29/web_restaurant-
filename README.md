<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Restaurante</title>
    <style>
        /* General */
        body {
            font-family: Arial, sans-serif;
            background-color: aqua;
            color: #333;
            margin: 0;
            padding: 0;
        }

        /* Header */
        header {
            background-color: #007BFF;
            color: white;
            text-align: center;
            padding: 20px;
        }

        header h1 {
            margin: 0;
            font-size: 2.5rem;
        }

        /* Main content */
        main {
            padding: 20px;
        }

        .main-image {
            display: block;
            margin: 20px auto;
            width: 60%;
            border-radius: 10px;
        }

        /* Gallery */
        .gallery {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
            gap: 10px;
            margin: 20px 0;
        }

        .gallery img {
            width: 100%;
            height: auto;
            border-radius: 5px;
            border: 2px solid #ccc;
            transition: transform 0.3s ease-in-out;
        }

        .gallery img:hover {
            transform: scale(1.1);
            border-color: #007BFF;
        }

        /* Video Gallery */
        .video-gallery {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
            gap: 10px;
        }

        video {
            width: 100%;
            border-radius: 5px;
            border: 2px solid #ccc;
            transition: transform 0.3s ease-in-out;
        }

        video:hover {
            transform: scale(1.1);
            border-color: #007BFF;
        }

        /* Form and Buttons */
        form, .login-form {
            margin-top: 20px;
        }

        label {
            font-weight: bold;
        }

        input, select, button {
            display: block;
            width: 100%;
            max-width: 300px;
            margin: 10px 0;
            padding: 10px;
            border: 2px solid #007BFF;
            border-radius: 5px;
            font-size: 1rem;
        }

        button {
            background-color: #FF5733;
            color: white;
            border: none;
            cursor: pointer;
            font-weight: bold;
        }

        button:hover {
            background-color: #C70039;
        }

        /* Footer */
        footer {
            background-color: #333;
            color: white;
            text-align: center;
            padding: 10px;
        }
    </style>
</head>
<body>
    <header>
        <h1>New Awesome Products</h1>
    </header>
    <main>
        <img class="main-image" src="https://media.istockphoto.com/id/139496979/es/foto/variedad-de-frutas-y-verduras-fondo.jpg?s=1024x1024&w=is&k=20&c=sZwklEAbKT7oshGDxjhIo8ZrSr2clUkIkzj8YNndKII=" alt="product image">
        <h2>Introducing our latest products, designed to make your life easier and more efficient.</h2>
        <ol>
            <li>Manzanas</li>
            <li>Papas</li>
            <li>Cebollas, platos y más</li>
        </ol>
        <section class="gallery">
            <h2>Galería de Platos</h2>
            <img src="Longaniza.jpg" alt="Plato de longaniza">
            <img src="Parrillada.jpg" alt="Parrillada del día">
            <img src="pechuga a la plancha.jpg" alt="Qué delicia de pechuga">
            <img src="pechuga a la crema.jpg" alt="Pechuga a la crema">
            <img src="salpicon de pulpo y camarones.jpg" alt="Ricos y sabrosos mariscos">
            <img src="Salami.jpg" alt="Salami a degustar">
        </section>
        <section>
            <h2>Video del Restaurante</h2>
            <div class="video-gallery">
                <video controls><source src="mofongo.mp4" type="video/mp4"></video>
                <video controls><source src="Alitas.mp4" type="video/mp4"></video>
                <video controls><source src="Longaniza1.mp4" type="video/mp4"></video>
                <video controls><source src="pechuga a la plancha.mp4" type="video/mp4"></video>
                <video controls><source src="Salami.mp4" type="video/mp4"></video>
                <video controls><source src="Pinchos.mp4" type="video/mp4"></video>
            </div>
        </section>
        <h2>Order now!</h2>
        <form>
            <label for="vegetales">Elige un Vegetal:</label>
            <select id="vegetales" name="vegetales">
                <option>Zanahoria</option>
                <option>Cebolla</option>
                <option>Ajo</option>
                <option>Aji</option>
                <option>Brocoli</option>
                <option>Remolacha</option>
                <option>Berro</option>
                <option>Espinaca</option>
                <option>Verduras</option>
                <option>Pimientos</option>
            </select>
            <br><br>
            <label for="frutas">Elige una Fruta:</label>
            <select id="frutas" name="frutas">
                <option>Bananas</option>
                <option>Uva</option>
                <option>Aguacates</option>
                <option>Manzana</option>
                <option>Sandía</option>
                <option>Guayaba</option>
                <option>Mango</option>
                <option>Chinola</option>
                <option>Pera</option>
                <option>Fresa</option>
            </select>
        </form>
        <div class="login-form">
            <label for="name">Name:</label>
            <input type="text" id="name" name="name" placeholder="Name">
            <label for="email">Email:</label>
            <input type="email" id="email" name="email" placeholder="Email">
            <button type="submit">Submit</button>
        </div>
    </main>
    <footer>
        <p>&copy; 2024 Henry Guzman y contenido by Jusset Vidal. Todos los derechos reservados.</p>
    </footer>
</body>
</html>
