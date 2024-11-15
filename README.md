<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sueños de Mermelada - Tienda</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <!-- Header -->
    <header>
        <h1>Sueños de Mermelada</h1>
        <nav>
            <a href="#home">Inicio</a>
            <a href="#products">Productos</a>
            <a href="#cart">Carrito</a>
        </nav>
    </header>

    <!-- Home Section -->
    <section id="home">
        <h2>Bienvenidos a Sueños de Mermelada</h2>
        <p>La mejor mermelada de guayaba hecha con amor y calidad.</p>
    </section>

    <!-- Products Section -->
    <section id="products">
        <h2>Nuestras Mermeladas</h2>
        <div class="product-list">
            <!-- Producto 1 -->
            <div class="product">
                <h3>Mermelada de Guayaba Clásica</h3>
                <p>Deliciosa y natural.</p>
                <p>Precio: Bs. 20</p>
                <button onclick="addToCart('Mermelada de Guayaba Clásica', 20)">Añadir al Carrito</button>
            </div>
            <!-- Producto 2 -->
            <div class="product">
                <h3>Mermelada de Guayaba con Jengibre</h3>
                <p>Un toque especial de jengibre.</p>
                <p>Precio: Bs. 25</p>
                <button onclick="addToCart('Mermelada de Guayaba con Jengibre', 25)">Añadir al Carrito</button>
            </div>
            <!-- Más productos se pueden agregar aquí -->
        </div>
    </section>

    <!-- Cart Section -->
    <section id="cart">
        <h2>Carrito de Compras</h2>
        <div id="cartItems"></div>
        <p id="totalPrice">Total: Bs. 0</p>
        <button onclick="checkout()">Ir a Pagar</button>
    </section>

    <!-- Checkout Section -->
    <section id="checkout" style="display: none;">
        <h2>Información de Pago</h2>
        <form>
            <label for="name">Nombre:</label>
            <input type="text" id="name" required>
            <label for="address">Dirección:</label>
            <input type="text" id="address" required>
            <label for="payment">Método de Pago:</label>
            <select id="payment">
                <option value="card">Tarjeta de Crédito</option>
                <option value="paypal">PayPal</option>
            </select>
            <button type="submit">Pagar</button>
        </form>
    </section>

    <script src="script.js"></script>
</body>
</html>
