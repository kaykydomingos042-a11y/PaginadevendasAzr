<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>AZR Marketing - Vendas</title>
    <style>
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background: linear-gradient(135deg, #2d1b69, #9d4edd);
            color: #ffffff;
            margin: 0;
            padding: 0;
            overflow-x: hidden;
            min-height: 100vh;
            animation: fadeIn 1s ease-in;
        }
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }
        .fadeOut {
            animation: fadeOut 0.5s ease-out forwards;
        }
        @keyframes fadeOut {
            from { opacity: 1; transform: translateY(0); }
            to { opacity: 0; transform: translateY(-20px); }
        }
        .neon-text {
            text-shadow: 0 0 10px #9d4edd, 0 0 20px #9d4edd, 0 0 30px #9d4edd;
        }
        header {
            text-align: center;
            padding: 30px;
            background: rgba(45, 27, 105, 0.9);
            border-bottom: 3px solid #9d4edd;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.3);
            animation: slideInFromTop 1s ease-out;
        }
        @keyframes slideInFromTop {
            from { transform: translateY(-50px); opacity: 0; }
            to { transform: translateY(0); opacity: 1; }
        }
        .product-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
            gap: 30px;
            padding: 40px;
            max-width: 1400px;
            margin: 0 auto;
            animation: slideInFromBottom 1s ease-out 0.5s both;
        }
        @keyframes slideInFromBottom {
            from { transform: translateY(50px); opacity: 0; }
            to { transform: translateY(0); opacity: 1; }
        }
        .product-card {
            background: rgba(45, 27, 105, 0.95);
            border: 3px solid #9d4edd;
            border-radius: 15px;
            padding: 25px;
            text-align: center;
            box-shadow: 0 0 30px #9d4edd;
            transition: transform 0.3s, box-shadow 0.3s;
            animation: cardFadeIn 1s ease-out both;
            animation-delay: calc(var(--delay) * 0.2s);
        }
        .product-card:nth-child(1) { --delay: 1; }
        .product-card:nth-child(2) { --delay: 2; }
        .product-card:nth-child(3) { --delay: 3; }
        @keyframes cardFadeIn {
            from { opacity: 0; transform: scale(0.9); }
            to { opacity: 1; transform: scale(1); }
        }
        .product-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 10px 40px #9d4edd;
        }
        .product-image {
            width: 100%;
            height: 250px;
            background: linear-gradient(135deg, #9d4edd, #2d1b69);
            margin-bottom: 15px;
            border-radius: 10px;
            display: flex;
            align-items: center;
            justify-content: center;
            color: #ffffff;
            font-size: 1.5em;
            font-weight: bold;
            box-shadow: inset 0 0 20px rgba(255, 255, 255, 0.1);
        }
        button {
            padding: 15px 30px;
            background: linear-gradient(135deg, #9d4edd, #2d1b69);
            border: none;
            color: #ffffff;
            font-weight: bold;
            font-size: 16px;
            cursor: pointer;
            border-radius: 8px;
            transition: all 0.3s;
        }
        button:hover {
            box-shadow: 0 0 20px #9d4edd;
            transform: scale(1.05);
        }
    </style>
</head>
<body>
    <header>
        <h1 class="neon-text">AZR Marketing</h1>
        <p class="neon-text">Produtos Exclusivos em Tema Hacking</p>
    </header>
    <div class="product-grid">
        <div class="product-card">
            <div class="product-image">Imagem do Produto 1</div>
            <h3 class="neon-text">Ferramenta de Análise de Rede</h3>
            <p>Descrição breve do produto. Ideal para profissionais de segurança.</p>
            <button onclick="document.body.classList.add('fadeOut'); setTimeout(() => window.location.href='venda-produto1.html', 500);">Comprar Agora</button>
        </div>
        <div class="product-card">
            <div class="product-image">Imagem do Produto 2</div>
            <h3 class="neon-text">Kit de Segurança Cibernética</h3>
            <p>Descrição breve do produto. Tudo que você precisa para proteger seus dados.</p>
            <button onclick="document.body.classList.add('fadeOut'); setTimeout(() => window.location.href='venda-produto2.html', 500);">Comprar Agora</button>
        </div>
        <div class="product-card">
            <div class="product-image">Imagem do Produto 3</div>
            <h3 class="neon-text">Curso de Hacking Ético</h3>
            <p>Descrição breve do produto. Aprenda com os melhores no mercado.</p>
            <button onclick="document.body.classList.add('fadeOut'); setTimeout(() => window.location.href='venda-produto3.html', 500);">Comprar Agora</button>
        </div>
        <!-- Adicione mais produtos conforme necessário -->
    </div>
</body>
</html>
