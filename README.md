# Frontend
// pagina principal
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8"> <!-- Configuración del conjunto de caracteres para UTF-8 -->
    <meta name="viewport" content="width=device-width, initial-scale=1.0"> <!-- Ajuste de la escala para dispositivos móviles -->
    <title>HACS</title> <!-- Título de la pestaña del navegador -->
</head>
<body>
    <h1>Hummanitarian Aid Coordination System </h1> <!-- Título visible en la página -->
    
    <!-- Etiqueta para una lista desplegable -->
    <label for="options">Select an option:</label>
    <select id="options" onchange="navigate()"> <!-- Lista desplegable, ejecuta la función `navigate` al cambiar la selección -->
        <option value="">--Select--</option> <!-- Opción por defecto -->
        <option value="login.html">Login Page</option> <!-- Redirige a `login.html` -->
        <option value="register.html">Register Page</option> <!-- Redirige a `register.html` -->
    </select>

    <script>
        // Función para redirigir según la selección
        function navigate() {
            const selectedOption = document.getElementById('options').value; // Obtiene el valor seleccionado
            if (selectedOption) { // Si se seleccionó una opción válida
                window.location.href = selectedOption; // Redirige al archivo correspondiente
            }
        }
    </script>
</body>
</html>

// pagina login
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Login Page</title>
</head>
<body>
    <h1>Login</h1>

    <!-- Form sends data to the server endpoint -->
    <form action="https://example.com/api/save-data" method="POST">
        <label for="username">Username:</label>
        <input type="text" id="username" name="username" required>
        <br><br>

        <label for="password">Password:</label>
        <input type="password" id="password" name="password" required>
        <br><br>

        <label for="id">ID:</label>
        <input type="text" id="id" name="user_id" required>
        <br><br>

        <button type="submit">Submit</button>
    </form>

    <!-- Button to return to the main page -->
    <button onclick="location.href='index.html'">Back to Main Page</button>
</body>
</html>


//pagina register
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Register Page</title>
</head>
<body>
    <h1>Register</h1>

    <!-- Form sends data to the server endpoint -->
    <form action="https://example.com/api/save-data" method="POST">
        <label for="username">Username:</label>
        <input type="text" id="username" name="username" required>
        <br><br>

        <label for="password">Password:</label>
        <input type="password" id="password" name="password" required>
        <br><br>

        <label for="id">ID:</label>
        <input type="text" id="id" name="user_id" required>
        <br><br>

        <button type="submit">Submit</button>
    </form>

    <!-- Button to return to the main page -->
    <button onclick="location.href='index.html'">Back to Main Page</button>
</body>
</html>
