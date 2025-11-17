<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<style>
    body {
        font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        background: #fdf6f9;
        color: #3c2a35;
        margin: 0;
    }

    .banner {
        width: 100%;
        text-align: center;
        margin: 20px 0;
    }

    .banner img {
        width: 220px;
        border-radius: 15px;
        box-shadow: 0 5px 15px rgba(0,0,0,0.1);
        transition: transform 0.3s;
    }

    .banner img:hover { transform: scale(1.05); }

    .produtos {
        padding: 40px 20px;
        text-align: center;
    }

    .produtos h2 {
        font-size: 30px;
        font-weight: 600;
        margin-bottom: 40px;
        color: #7d4c70;
    }

    .grid-produtos {
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
        gap: 25px;
        max-width: 1200px;
        margin: 0 auto;
    }

    .item {
        background: #ffffff;
        border-radius: 15px;
        padding: 20px;
        box-shadow: 0 8px 20px rgba(0,0,0,0.08);
        transition: transform 0.3s, box-shadow 0.3s;
    }

    .item:hover {
        transform: translateY(-5px);
        box-shadow: 0 15px 25px rgba(0,0,0,0.12);
    }

    .item img {
        width: 100%;
        height: 300px; /* maior tamanho */
        object-fit: contain; /* ajusta a imagem inteira dentro do quadrado */
        border-radius: 12px;
        margin-bottom: 10px;
        background: #f8f3f8; /* fundo leve para destacar imagens menores */
    }

    .item h3 { 
        font-size: 14px; /* descrição menor */
        margin-bottom: 8px; 
        min-height: 40px; 
    }

    .btn {
        display: inline-block;
        padding: 12px 20px;
        margin-top: 10px;
        background: #9b5fbf; /* roxo mais claro */
        color: #fff;
        text-decoration: none;
        border-radius: 10px;
        font-weight: 500;
        cursor: pointer;
        transition: background 0.3s, transform 0.2s;
    }

    .btn:hover {
        background: #7d4c70; /* escurece no hover */
        transform: scale(1.05);
    }

    /* CARRINHO FLUTUANTE */
    #cart-btn {
        position: fixed;
        bottom: 20px;
        right: 20px;
        background: #9b5fbf; /* mesma cor do btn comprar */
        color: white;
        width: 55px;
        height: 55px;
        border-radius: 50%;
        display: flex;
        align-items: center;
        justify-content: center;
        font-size: 26px;
        cursor: pointer;
        box-shadow: 0 5px 15px rgba(0,0,0,0.2);
        z-index: 1000;
        transition: transform 0.2s;
    }

    #cart-btn:hover { transform: scale(1.1); }

    #cart-count {
        position: absolute;
        top: -5px;
        right: -5px;
        background: #ff3b5c;
        color: white;
        font-size: 14px;
        width: 22px;
        height: 22px;
        border-radius: 50%;
        display: flex;
        align-items: center;
        justify-content: center;
    }

    /* CARRINHO DESLIZANTE */
    #cart {
        position: fixed;
        right: -100%;
        top: 0;
        width: 320px;
        max-width: 90%;
        height: 100%;
        background: #fff;
        box-shadow: -5px 0 25px rgba(0,0,0,0.15);
        padding: 20px;
        transition: right 0.3s ease-in-out;
        z-index: 999;
        overflow-y: auto;
    }

    #cart.active { right: 0; }

    #cart h2 { color: #7d4c70; margin-bottom: 20px; }
    .cart-item { display: flex; justify-content: space-between; margin-bottom: 15px; }
    .cart-item span { font-size: 16px; }
    .cart-buttons { margin-top: 20px; display: flex; gap: 10px; }
    .cart-buttons .btn { flex: 1; }

    /* Botão fechar do carrinho */
    #close-cart {
        position: absolute;
        top: 15px;
        right: 15px;
        background: #fff;
        color: #000;
        border: none;
        font-size: 20px;
        width: 35px;
        height: 35px;
        border-radius: 50%;
        cursor: pointer;
        display: flex;
        align-items: center;
        justify-content: center;
        z-index: 1001;
    }

    @media (max-width: 768px) {
        .grid-produtos { grid-template-columns: repeat(2, 1fr); }
        .produtos h2 { font-size: 24px; }
    }

    @media (max-width: 480px) {
        .grid-produtos { grid-template-columns: repeat(2, 1fr); }
        .produtos h2 { font-size: 22px; }
    }
</style>
</head>
<body>

<div class="banner">
    <img src="https://i.imgur.com/sGmHrFU.jpg" alt="Banner Camila Perfumaria">
</div>

<section class="produtos">
    <h2>Produtos Disponíveis na Beauty Week</h2>
    <div class="grid-produtos">

        <div class="item" data-name="Coffee Woman Unique Floriental Gourmand" data-link="https://wa.me/5519989448747?text=Coffee%20Woman%20Unique%20Floriental%20Gourmand">
            <img src="https://i.postimg.cc/9fj2CMyN/Whats-App-Image-2025-11-16-at-21-50-17.jpg" alt="Coffee Woman">
            <h3>Coffee Woman Unique Floriental Gourmand Desodorante Colônia 100ml</h3>
            <button class="btn add-cart">Comprar</button>
        </div>

        <div class="item" data-name="Clash Desodorante Colônia" data-link="https://wa.me/5519989448747?text=Clash%20Desodorante%20Colônia">
            <img src="https://i.postimg.cc/mrG4BD7d/Whats-App-Image-2025-11-16-at-22-18-38.jpg" alt="Clash">
            <h3>Clash Desodorante Colônia 100ml</h3>
            <button class="btn add-cart">Comprar</button>
        </div>

        <div class="item" data-name="Malbec Icon" data-link="https://wa.me/5519989448747?text=Malbec%20Icon">
            <img src="https://i.postimg.cc/6QNKt3CM/Whats-App-Image-2025-11-16-at-22-18-38-(1).jpg" alt="Malbec Icon">
            <h3>Malbec Icon Desodorante Colônia 100ml</h3>
            <button class="btn add-cart">Comprar</button>
        </div>

        <div class="item" data-name="Combo Siàge Shampoo + Condicionador" data-link="https://wa.me/5519989448747?text=Combo%20Siàge%20Shampoo%20+%20Condicionador">
            <img src="https://i.postimg.cc/LsMS2XjD/Whats-App-Image-2025-11-16-at-22-18-38-(2).jpg" alt="Combo Siàge">
            <h3>Combo Siàge Acelera o Crescimento: Shampoo 250ml + Condicionador 200ml</h3>
            <button class="btn add-cart">Comprar</button>
        </div>

        <div class="item" data-name="Spray Perfumado e Sabonete Instance" data-link="https://wa.me/5519989448747?text=Spray%20Perfumado%20e%20Sabonete%20Instance">
            <img src="https://i.postimg.cc/N0wtBMRk/Whats-App-Image-2025-11-16-at-22-18-38-(3).jpg" alt="Spray Perfumado">
            <h3>Spray Perfumado e Sabonete Vegetal em Barra Instance Morango Irresistível</h3>
            <button class="btn add-cart">Comprar</button>
        </div>

        <div class="item" data-name="Boti Baby Colônia do Sol" data-link="https://wa.me/5519989448747?text=Boti%20Baby%20Colônia%20do%20Sol">
            <img src="https://i.postimg.cc/3wHhYR2g/Whats-App-Image-2025-11-16-at-22-18-38-(4).jpg" alt="Boti Baby">
            <h3>Boti Baby Colônia do Sol 100ml</h3>
            <button class="btn add-cart">Comprar</button>
        </div>

        <div class="item" data-name="Sabonete Líquido Boti Baby" data-link="https://wa.me/5519989448747?text=Sabonete%20Líquido%20Boti%20Baby">
            <img src="https://i.postimg.cc/6pZKkR4b/Whats-App-Image-2025-11-16-at-22-18-38-(5).jpg" alt="Sabonete Líquido">
            <h3>Sabonete Líquido de Glicerina Boti Baby 200ml</h3>
            <button class="btn add-cart">Comprar</button>
        </div>

        <div class="item" data-name="Colônia Velvet Sensual Intense" data-link="https://wa.me/5519989448747?text=Colônia%20Velvet%20Sensual%20Intense">
            <img src="https://i.postimg.cc/Z5NmG3vw/Whats-App-Image-2025-11-16-at-22-18-39.jpg" alt="Velvet Sensual">
            <h3>Colônia Velvet Sensual Intense 100ml</h3>
            <button class="btn add-cart">Comprar</button>
        </div>

        <div class="item" data-name="Ilía Secreto 50 ml" data-link="https://wa.me/5519989448747?text=Ilía%20Secreto%2050ml">
            <img src="https://i.postimg.cc/7YdDtXhG/Whats-App-Image-2025-11-16-at-22-25-37.jpg" alt="Ilía Secreto">
            <h3>Ilía Secreto 50 ml</h3>
            <button class="btn add-cart">Comprar</button>
        </div>

        <div class="item" data-name="Kriska Shock 100 ml" data-link="https://wa.me/5519989448747?text=Ilía%20Secreto%2050ml">
            <img src="https://i.postimg.cc/HkMmq58V/Whats-App-Image-2025-11-16-at-22-25-36-(1).jpg" alt="Kriska Shock 100 ml">
            <h3>Kriska Shock 100 ml</h3>
            <button class="btn add-cart">Comprar</button>
        </div>
	
	<div class="item" data-name="Desodorante Body Spray Imensi 100ml" data-link="https://wa.me/5519989448747?text=Ilía%20Secreto%2050ml">
            <img src="https://i.postimg.cc/KYHc9Yhh/Whats-App-Image-2025-11-16-at-22-36-41.jpg" alt="Desodorante Body Spray Imensi 100ml">
            <h3>Desodorante Body Spray Imensi 100ml</h3>
            <button class="btn add-cart">Comprar</button>
        </div>

	<div class="item" data-name="Loção Hidratante e Sabonete Cuide-Bem Cereja Livre" data-link="https://wa.me/5519989448747?text=Ilía%20Secreto%2050ml">
            <img src="https://i.postimg.cc/g2hpCRL2/Whats-App-Image-2025-11-16-at-22-18-40-(2).jpg" alt="Loção Hidratante e Sabonete Cuide-Bem Cereja Livre">
            <h3>Loção Hidratante e Sabonete Cuide-Bem Cereja Livre</h3>
            <button class="btn add-cart">Comprar</button>
        </div>

	<div class="item" data-name="Coffee Man Unique Fougère Oriental Colônia 100ml" data-link="https://wa.me/5519989448747?text=Ilía%20Secreto%2050ml">
            <img src="https://i.postimg.cc/FHSvMckJ/Whats-App-Image-2025-11-16-at-22-18-40-(1).jpg" alt="Coffee Man Unique Fougère Oriental Colônia 100ml">
            <h3>Coffee Man Unique Fougère Oriental Colônia 100ml</h3>
            <button class="btn add-cart">Comprar</button>
        </div>
	
	<div class="item" data-name="Sabonete Líquido Cuide-se Bem Melissa 150ml" data-link="https://wa.me/5519989448747?text=Ilía%20Secreto%2050ml">
            <img src="https://i.postimg.cc/y8RKM93R/Whats-App-Image-2025-11-16-at-22-18-40.jpg" alt="Sabonete Líquido Cuide-se Bem Melissa 150ml">
            <h3>Sabonete Líquido Cuide-se Bem Melissa 150ml</h3>
            <button class="btn add-cart">Comprar</button>
        </div>

	<div class="item" data-name="Batom Vermelho 310 Cremoso" data-link="https://wa.me/5519989448747?text=Ilía%20Secreto%2050ml">
            <img src="https://i.postimg.cc/Y2yN16sC/Whats-App-Image-2025-11-16-at-22-36-41-(1).jpg" alt="Batom Vermelho 310 Cremoso">
            <h3>Batom Vermelho 310 Cremoso</h3>
            <button class="btn add-cart">Comprar</button>
        </div>

	<div class="item" data-name="Batom Líquido Niina Secrets Skinny Matte" data-link="https://wa.me/5519989448747?text=Ilía%20Secreto%2050ml">
            <img src="https://i.postimg.cc/T2mmWznX/Whats-App-Image-2025-11-16-at-22-36-42.jpg" alt="Batom Líquido Niina Secrets Skinny Matte">
            <h3>Batom Líquido Niina Secrets Skinny Matte</h3>
            <button class="btn add-cart">Comprar</button>
        </div>

	<div class="item" data-name="Combo Creme Hidratante Desodorante Indulgent Cream 100ml + Body Spray Eudora 100ml" data-link="https://wa.me/5519989448747?text=Ilía%20Secreto%2050ml">
            <img src="https://i.postimg.cc/T3bxzm5c/Whats-App-Image-2025-11-16-at-22-18-39-(2).jpg" alt="Combo Creme Hidratante Desodorante Indulgent Cream 100ml + Body Spray Eudora 100ml">
            <h3>Combo Creme Hidratante Desodorante Indulgent Cream 100ml + Body Spray Eudora 100ml</h3>
            <button class="btn add-cart">Comprar</button>
        </div>

	<div class="item" data-name="Condicionador Siàge Expert Regeneração Pós Química 200ml" data-link="https://wa.me/5519989448747?text=Ilía%20Secreto%2050ml">
            <img src="https://i.postimg.cc/vTzZttQL/Whats-App-Image-2025-11-16-at-22-36-42-(1).jpg" alt="Condicionador Siàge Expert Regeneração Pós Química 200ml">
            <h3>Condicionador Siàge Expert Regeneração Pós Química 200ml</h3>
            <button class="btn add-cart">Comprar</button>
        </div>

	<div class="item" data-name="Condicionador Siàge Nutri Óleos Poderosos 200ml" data-link="https://wa.me/5519989448747?text=Ilía%20Secreto%2050ml">
            <img src="https://i.postimg.cc/d0vNzRvq/Whats-App-Image-2025-11-16-at-22-36-42-(2).jpg" alt="Condicionador Siàge Nutri Óleos Poderosos 200ml">
            <h3>Condicionador Siàge Nutri Óleos Poderosos 200ml</h3>
            <button class="btn add-cart">Comprar</button>
        </div>

	<div class="item" data-name="Refil Máscara Capilar Siàge Cica-Therapy 250g" data-link="https://wa.me/5519989448747?text=Ilía%20Secreto%2050ml">
            <img src="https://i.postimg.cc/BvQkj5yJ/Whats-App-Image-2025-11-16-at-22-36-42-(3).jpg" alt="Refil Máscara Capilar Siàge Cica-Therapy 250g">
            <h3>Refil Máscara Capilar Siàge Cica-Therapy 250g</h3>
            <button class="btn add-cart">Comprar</button>
        </div>

	<div class="item" data-name="Sabonetes em Barra Sortidos Cuide-se Bem 4x80g" data-link="https://wa.me/5519989448747?text=Ilía%20Secreto%2050ml">
            <img src="https://i.postimg.cc/pdhQcp5Y/Whats-App-Image-2025-11-16-at-22-36-42-(4).jpg" alt="Sabonetes em Barra Sortidos Cuide-se Bem 4x80g">
            <h3>Sabonetes em Barra Sortidos Cuide-se Bem 4x80g</h3>
            <button class="btn add-cart">Comprar</button>
        </div>

	<div class="item" data-name="Liz Flora Colônia" data-link="https://wa.me/5519989448747?text=Ilía%20Secreto%2050ml">
            <img src="https://i.postimg.cc/MK3QkzSr/Whats-App-Image-2025-11-16-at-22-36-42-(5).jpg" alt="Liz Flora Colônia">
            <h3>Liz Flora Colônia</h3>
            <button class="btn add-cart">Comprar</button>
        </div>	

	<div class="item" data-name="Kit Presente Floratta (3 itens)" data-link="https://wa.me/5519989448747?text=Ilía%20Secreto%2050ml">
            <img src="https://i.postimg.cc/B6NvxCZj/Whats-App-Image-2025-11-16-at-22-36-42-(6).jpg" alt="Kit Presente Floratta (3 itens)">
            <h3>Kit Presente Floratta (3 itens)</h3>
            <button class="btn add-cart">Comprar</button>
        </div>

    </div>
</section>

<div id="cart-btn">
    🛒
    <div id="cart-count">0</div>
</div>

<div id="cart">
    <button id="close-cart">✖</button>
    <h2>Seu Carrinho</h2>
    <div id="cart-items"></div>
    <div class="cart-buttons">
        <button class="btn" id="clear-cart">Limpar</button>
        <button class="btn" id="checkout">Finalizar</button>
    </div>
</div>

<script>
    const cartBtn = document.getElementById('cart-btn');
    const cart = document.getElementById('cart');
    const cartItemsContainer = document.getElementById('cart-items');
    const cartCount = document.getElementById('cart-count');
    const clearCartBtn = document.getElementById('clear-cart');
    const checkoutBtn = document.getElementById('checkout');
    const closeCartBtn = document.getElementById('close-cart');

    let cartItems = [];

    cartBtn.addEventListener('click', () => { cart.classList.toggle('active'); });
    closeCartBtn.addEventListener('click', () => { cart.classList.remove('active'); });

    document.querySelectorAll('.add-cart').forEach(btn => {
        btn.addEventListener('click', () => {
            const itemDiv = btn.closest('.item');
            const name = itemDiv.dataset.name;
            const link = itemDiv.dataset.link;
            cartItems.push({name, link});
            updateCart();
        });
    });

    function updateCart() {
        cartItemsContainer.innerHTML = '';
        cartItems.forEach((item, index) => {
            const div = document.createElement('div');
            div.classList.add('cart-item');
            div.innerHTML = `
                <span>${item.name}</span>
                <span style="cursor:pointer;" onclick="removeItem(${index})">❌</span>
            `;
            cartItemsContainer.appendChild(div);
        });
        cartCount.textContent = cartItems.length;
    }

    window.removeItem = function(index) {
        cartItems.splice(index, 1);
        updateCart();
    }

    clearCartBtn.addEventListener('click', () => {
        cartItems = [];
        updateCart();
    });

    checkoutBtn.addEventListener('click', () => {
        if(cartItems.length === 0){
            alert("Seu carrinho está vazio!");
            return;
        }
        let message = "Olá,%20quero%20comprar:%0A";
        cartItems.forEach(item => { message += "- " + item.name + "%0A"; });
        window.open("https://wa.me/5519989448747?text=" + message, "_blank");
    });
</script>

</body>
</html>
