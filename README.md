<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<style>
    body {
        margin: 0;
        font-family: Arial, sans-serif;
        background: #f7e9f3;
        color: #3c2a35;
    }

    /* BANNER */
    .banner {
        width: 100%;
        text-align: center;
        margin: 20px 0;
    }

    .banner img {
        width: 210px; /* AJUSTADO PARA FICAR PEQUENO */
        height: auto;
        display: block;
        margin: 0 auto;
        border-radius: 10px;
    }

    /* SEÇÃO PRODUTOS */
    .produtos {
        padding: 40px 20px;
        text-align: center;
    }

    .produtos h2 {
        font-size: 28px;
        margin-bottom: 30px;
    }

    .grid-produtos {
        display: grid;
        grid-template-columns: repeat(3, 1fr); /* 3 POR FILEIRA */
        gap: 25px;
        max-width: 1100px;
        margin: 0 auto;
    }

    .item {
        background: white;
        padding: 15px;
        border-radius: 12px;
        box-shadow: 0 2px 5px rgba(0,0,0,0.1);
        transition: 0.3s;
    }

    .item:hover {
        transform: scale(1.05);
    }

    .item img {
        width: 100%;
        height: auto;
        object-fit: contain;
        border-radius: 10px;
    }

    .item h3 {
        margin-top: 10px;
        font-size: 20px;
    }

    .item p {
        margin: 5px 0 10px;
    }

    .whatsapp {
        display: block;
        margin-top: 10px;
        padding: 10px;
        background: #7d4c70;
        color: white;
        text-decoration: none;
        border-radius: 8px;
        transition: 0.3s;
    }

    .whatsapp:hover {
        background: #a06b93;
    }

    /* RESPONSIVO CELULAR */
    @media (max-width: 768px) {
        .grid-produtos {
            grid-template-columns: 1fr 1fr;
        }
    }

    @media (max-width: 480px) {
        .grid-produtos {
            grid-template-columns: 1fr;
        }
    }
</style>
</head>
<body>

<!-- BANNER -->
<div class="banner">
    <img src="https://i.imgur.com/sGmHrFU.jpg" alt="Banner Camila Perfumaria">
</div>

<!-- PRODUTOS -->
<section class="produtos">
    <h2>Produtos Disponíveis na Beauty Week</h2>

    <div class="grid-produtos">

        <!-- PRODUTO 1 -->
        <div class="item">
            <img src="https://i.postimg.cc/9fj2CMyN/Whats-App-Image-2025-11-16-at-21-50-17.jpg" alt="Produto 1">
            <h3>Coffee Woman Unique Floriental Gourmand Desodorante Colônia 100ml</h3>
            <a class="whatsapp" href="https://wa.me/5519989448747?text=Olá,%20quero%20saber%20sobre%20o%20Coffee Woman Unique Floriental Gourmand Desodorante Colônia 100ml%20">Comprar</a>
        </div>

        <!-- PRODUTO 2 -->
        <div class="item">
            <img src="https://i.postimg.cc/mrG4BD7d/Whats-App-Image-2025-11-16-at-22-18-38.jpg" alt="Produto 2">
            <h3>Clash Desodorante Colônia 100ml</h3>
            <a class="whatsapp" href="https://wa.me/5519989448747?text=Olá,%20quero%20saber%20sobre%20o%20Clash Desodorante Colônia 100ml%20">Comprar</a>
        </div>

        <!-- PRODUTO 3 -->
        <div class="item">
            <img src="https://i.postimg.cc/6QNKt3CM/Whats-App-Image-2025-11-16-at-22-18-38-(1).jpg" alt="Produto 3">
            <h3>Malbec Icon Desodorante Colônia 100ml</h3>
            <a class="whatsapp" href="https://wa.me/5519989448747?text=Olá,%20quero%20saber%20sobre%20o%20Malbec Icon Desodorante Colônia 100ml%20">Comprar</a>
        </div>

	<!-- PRODUTO 4 -->
        <div class="item">
            <img src="https://i.postimg.cc/LsMS2XjD/Whats-App-Image-2025-11-16-at-22-18-38-(2).jpg" alt="Produto 4">
            <h3>Combo Siàge Acelera o Crescimento: Shampoo 250ml + Condicionador 200ml</h3>
            <a class="whatsapp" href="https://wa.me/5519989448747?text=Olá,%20quero%20saber%20sobre%20o%20Combo Siàge Acelera o Crescimento: Shampoo 250ml + Condicionador 200ml%20">Comprar</a>
        </div>
	
	<!-- PRODUTO 5 -->
        <div class="item">
            <img src="https://i.postimg.cc/N0wtBMRk/Whats-App-Image-2025-11-16-at-22-18-38-(3).jpg" alt="Produto 2">
            <h3>Spray Perfumado e Sabonete Vegetal em Barra Instance Morango Irresistível</h3>
            <a class="whatsapp" href="https://wa.me/5519989448747?text=Olá,%20quero%20saber%20sobre%20o%20Spray Perfumado e Sabonete Vegetal em Barra Instance Morango Irresistível%20">Comprar</a>
        </div>

	<!-- PRODUTO 6 -->
        <div class="item">
            <img src="https://i.postimg.cc/3wHhYR2g/Whats-App-Image-2025-11-16-at-22-18-38-(4).jpg" alt="Produto 3">
            <h3>Boti Baby Colônia do Sol 100ml</h3>
            <a class="whatsapp" href="https://wa.me/5519989448747?text=Olá,%20quero%20saber%20sobre%20o%20Boti Baby Colônia do Sol 100ml%20">Comprar</a>
        </div>

	<!-- PRODUTO 7 -->
        <div class="item">
            <img src="https://i.postimg.cc/6pZKkR4b/Whats-App-Image-2025-11-16-at-22-18-38-(5).jpg" alt="Produto 3">
            <h3>Sabonete Líquido de Glicerina Boti Baby 200ml</h3>
            <a class="whatsapp" href="https://wa.me/5519989448747?text=Olá,%20quero%20saber%20sobre%20o%20Sabonete Líquido de Glicerina Boti Baby 200ml%20">Comprar</a>
        </div>

	<!-- PRODUTO 8 -->
        <div class="item">
            <img src="https://i.postimg.cc/Z5NmG3vw/Whats-App-Image-2025-11-16-at-22-18-39.jpg" alt="Produto 3">
            <h3>Colônia Velvet Sensual Intense 100ml</h3>
            <a class="whatsapp" href="https://wa.me/5519989448747?text=Olá,%20quero%20saber%20sobre%20o%20Colônia Velvet Sensual Intense 100ml%20">Comprar</a>
        </div>

	<!-- PRODUTO 9 -->
        <div class="item">
            <img src="https://i.postimg.cc/7YdDtXhG/Whats-App-Image-2025-11-16-at-22-25-37.jpg" alt="Produto 3">
            <h3>Ilía Secreto 50 ml</h3>
            <a class="whatsapp" href="https://wa.me/5519989448747?text=Olá,%20quero%20saber%20sobre%20o%20Ilía Secreto 50 ml%20">Comprar</a>
        </div>

	<!-- PRODUTO 10 -->
        <div class="item">
            <img src="https://i.postimg.cc/P5DHgZvf/Whats-App-Image-2025-11-16-at-22-25-36-(2).jpg" alt="Produto 3">
            <h3>Ilía 50 ml</h3>
            <a class="whatsapp" href="https://wa.me/5519989448747?text=Olá,%20quero%20saber%20sobre%20o%20Ilía 50 ml%20">Comprar</a>
        </div>

	<!-- PRODUTO 11 -->
        <div class="item">
            <img src="https://i.postimg.cc/HkMmq58V/Whats-App-Image-2025-11-16-at-22-25-36-(1).jpg" alt="Produto 3">
            <h3>Kriska Shock 100 ml</h3>
            <a class="whatsapp" href="https://wa.me/5519989448747?text=Olá,%20quero%20saber%20sobre%20o%20Kriska Shock 100 ml%20">Comprar</a>
        </div>

	<!-- PRODUTO 12 -->
        <div class="item">
            <img src="https://i.postimg.cc/KYHc9Yhh/Whats-App-Image-2025-11-16-at-22-36-41.jpg" alt="Produto 3">
            <h3>Desodorante Body Spray Imensi 100ml</h3>
            <a class="whatsapp" href="https://wa.me/5519989448747?text=Olá,%20quero%20saber%20sobre%20o%20Desodorante Body Spray Imensi 100ml%20">Comprar</a>
        </div>

	<!-- PRODUTO 13 -->
        <div class="item">
            <img src="https://i.postimg.cc/g2hpCRL2/Whats-App-Image-2025-11-16-at-22-18-40-(2).jpg" alt="Produto 3">
            <h3>Loção Hidratante e Sabonete Cuide-Bem Cereja Livre</h3>
            <a class="whatsapp" href="https://wa.me/5519989448747?text=Olá,%20quero%20saber%20sobre%20o%20Hidratante e Sabonete Cuide-Bem Cereja Livre%20">Comprar</a>
        </div>

	<!-- PRODUTO 14 -->
        <div class="item">
            <img src="https://i.postimg.cc/FHSvMckJ/Whats-App-Image-2025-11-16-at-22-18-40-(1).jpg" alt="Produto 3">
            <h3>Coffee Man Unique Fougère Oriental Colônia 100ml</h3>
            <a class="whatsapp" href="https://wa.me/5519989448747?text=Olá,%20quero%20saber%20sobre%20o%20Coffee Man Unique Fougère Oriental Colônia 100ml%20">Comprar</a>
        </div>

	<!-- PRODUTO 15 -->
        <div class="item">
            <img src="https://i.postimg.cc/y8RKM93R/Whats-App-Image-2025-11-16-at-22-18-40.jpg" alt="Produto 3">
            <h3>Sabonete Líquido Cuide-se Bem Melissa 150ml</h3>
            <a class="whatsapp" href="https://wa.me/5519989448747?text=Olá,%20quero%20saber%20sobre%20o%20Sabonete Líquido Cuide-se Bem Melissa 150ml%20">Comprar</a>
        </div>

	<!-- PRODUTO 16 -->
        <div class="item">
            <img src="https://i.postimg.cc/Y2yN16sC/Whats-App-Image-2025-11-16-at-22-36-41-(1).jpg" alt="Produto 3">
            <h3>Batom Vermelho 310 Cremoso</h3>
            <a class="whatsapp" href="https://wa.me/5519989448747?text=Olá,%20quero%20saber%20sobre%20o%20Batom Vermelho 310 Cremoso%20">Comprar</a>
        </div>

	<!-- PRODUTO 17 -->
        <div class="item">
            <img src="https://i.postimg.cc/T2mmWznX/Whats-App-Image-2025-11-16-at-22-36-42.jpg" alt="Produto 3">
            <h3>Batom Líquido Niina Secrets Skinny Matte</h3>
            <a class="whatsapp" href="https://wa.me/5519989448747?text=Olá,%20quero%20saber%20sobre%20o%20Batom Líquido Niina Secrets Skinny Matte%20">Comprar</a>
        </div>

	<!-- PRODUTO 18 -->
        <div class="item">
            <img src="https://i.postimg.cc/T3bxzm5c/Whats-App-Image-2025-11-16-at-22-18-39-(2).jpg" alt="Produto 3">
            <h3>Combo Creme Hidratante Desodorante Indulgent Cream 100ml + Body Spray Eudora 100ml</h3>
            <a class="whatsapp" href="https://wa.me/5519989448747?text=Olá,%20quero%20saber%20sobre%20o%20Combo Creme Hidratante Desodorante Indulgent Cream 100ml + Body Spray Eudora 100ml%20">Comprar</a>
        </div>

	<!-- PRODUTO 19 -->
        <div class="item">
            <img src="https://i.postimg.cc/vTzZttQL/Whats-App-Image-2025-11-16-at-22-36-42-(1).jpg" alt="Produto 3">
            <h3>Condicionador Siàge Expert Regeneração Pós Química 200ml</h3>
            <a class="whatsapp" href="https://wa.me/5519989448747?text=Olá,%20quero%20saber%20sobre%20o%20Condicionador Siàge Expert Regeneração Pós Química 200ml%20">Comprar</a>
        </div>

	<!-- PRODUTO 20 -->
        <div class="item">
            <img src="https://i.postimg.cc/d0vNzRvq/Whats-App-Image-2025-11-16-at-22-36-42-(2).jpg" alt="Produto 3">
            <h3>Condicionador Siàge Nutri Óleos Poderosos 200ml</h3>
            <a class="whatsapp" href="https://wa.me/5519989448747?text=Olá,%20quero%20saber%20sobre%20o%20Condicionador Siàge Nutri Óleos Poderosos 200ml%20">Comprar</a>
        </div>

	<!-- PRODUTO 21 -->
        <div class="item">
            <img src="https://i.postimg.cc/BvQkj5yJ/Whats-App-Image-2025-11-16-at-22-36-42-(3).jpg" alt="Produto 3">
            <h3>Refil Máscara Capilar Siàge Cica-Therapy 250g</h3>
            <a class="whatsapp" href="https://wa.me/5519989448747?text=Olá,%20quero%20saber%20sobre%20o%20Refil Máscara Capilar Siàge Cica-Therapy 250g%20">Comprar</a>
        </div>

	<!-- PRODUTO 22 -->
        <div class="item">
            <img src="https://i.postimg.cc/pdhQcp5Y/Whats-App-Image-2025-11-16-at-22-36-42-(4).jpg" alt="Produto 3">
            <h3>Sabonetes em Barra Sortidos Cuide-se Bem 4x80g</h3>
            <a class="whatsapp" href="https://wa.me/5519989448747?text=Olá,%20quero%20saber%20sobre%20o%20Sabonetes em Barra Sortidos Cuide-se Bem 4x80g%20">Comprar</a>
        </div>

	<!-- PRODUTO 23 -->
        <div class="item">
            <img src="https://i.postimg.cc/MK3QkzSr/Whats-App-Image-2025-11-16-at-22-36-42-(5).jpg" alt="Produto 3">
            <h3>Liz Flora Colônia</h3>
            <a class="whatsapp" href="https://wa.me/5519989448747?text=Olá,%20quero%20saber%20sobre%20o%20Liz Flora Colônia%20">Comprar</a>
        </div>

	<!-- PRODUTO 24 -->
        <div class="item">
            <img src="https://i.postimg.cc/B6NvxCZj/Whats-App-Image-2025-11-16-at-22-36-42-(6).jpg" alt="Produto 3">
            <h3>Kit Presente Floratta (3 itens)</h3>
            <a class="whatsapp" href="https://wa.me/5519989448747?text=Olá,%20quero%20saber%20sobre%20o%20Kit Presente Floratta (3 itens)%20">Comprar</a>
        </div>

    </div>
</section>

</body>
</html>
