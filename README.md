# vale-roleplay-site
<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Venda - Vale Roleplay MTA</title>
  <style>
    @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;600&display=swap');

    body {
      margin: 0;
      font-family: 'Poppins', sans-serif;
      background: #1e003e; /* roxo escuro */
      color: #ddd;
      overflow-x: hidden;
      position: relative;
      min-height: 100vh;
    }

    /* Fundo "Vale Roleplay" grande e transparente */
    body::before {
      content: "Vale Roleplay";
      position: fixed;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
      font-size: 10vw;
      font-weight: 900;
      color: rgba(128, 0, 255, 0.1);
      user-select: none;
      pointer-events: none;
      z-index: 0;
      white-space: nowrap;
      font-family: 'Poppins', sans-serif;
      letter-spacing: 0.3em;
    }

    header {
      background: #4b0082;
      padding: 1.5rem 2rem;
      text-align: center;
      font-size: 2rem;
      font-weight: 600;
      color: #f0e6ff;
      letter-spacing: 0.05em;
      position: relative;
      z-index: 2;
      box-shadow: 0 2px 8px rgba(0,0,0,0.6);
    }

    main {
      max-width: 960px;
      margin: 2rem auto 4rem auto;
      padding: 0 1rem;
      position: relative;
      z-index: 2;
    }

    h2 {
      color: #bb86fc;
      margin-bottom: 1rem;
      border-bottom: 2px solid #bb86fc;
      padding-bottom: 0.5rem;
      font-weight: 600;
    }

    section {
      background: #320a5c;
      border-radius: 12px;
      padding: 1.5rem 2rem;
      margin-bottom: 2rem;
      box-shadow: 0 0 10px rgba(187, 134, 252, 0.3);
      transition: box-shadow 0.3s ease;
    }
    section:hover {
      box-shadow: 0 0 15px rgba(187, 134, 252, 0.7);
    }

    .product {
      display: flex;
      justify-content: space-between;
      align-items: center;
      margin-bottom: 1.2rem;
      border-bottom: 1px solid #5e2ea2;
      padding-bottom: 0.8rem;
    }
    .product:last-child {
      border-bottom: none;
    }

    .product-name {
      font-weight: 600;
      font-size: 1.1rem;
    }
    .product-desc {
      font-size: 0.9rem;
      color: #b3a0ff;
    }
    .product-price {
      font-weight: 700;
      color: #dda0ff;
      font-size: 1.1rem;
      min-width: 70px;
      text-align: right;
    }

    button.buy-btn {
      background: #9b59b6;
      color: white;
      border: none;
      padding: 0.5rem 1.2rem;
      border-radius: 6px;
      cursor: pointer;
      font-weight: 600;
      font-size: 1rem;
      transition: background-color 0.25s ease;
      margin-left: 1rem;
    }
    button.buy-btn:hover {
      background: #7e3fbf;
    }

    footer {
      text-align: center;
      padding: 1rem 0;
      color: #8c7ae6;
      font-size: 0.9rem;
      border-top: 1px solid #4b0082;
      position: relative;
      z-index: 2;
    }

    /* Responsividade simples */
    @media (max-width: 600px) {
      .product {
        flex-direction: column;
        align-items: flex-start;
      }
      .product-price, button.buy-btn {
        margin-top: 0.5rem;
        text-align: left;
        min-width: auto;
      }
    }
  </style>
</head>
<body>
  <header>Vale Roleplay - Loja Oficial</header>
  <main>
    <section id="faccoes">
      <h2>Facções</h2>
      <div class="product">
        <div>
          <div class="product-name">Facção - Polícia</div>
          <div class="product-desc">Ganhe acesso VIP a polícia e comandos exclusivos</div>
        </div>
        <div>
          <span class="product-price">R$ 25,00</span>
          <button class="buy-btn">Comprar</button>
        </div>
      </div>
      <div class="product">
        <div>
          <div class="product-name">Facção - Máfia</div>
          <div class="product-desc">Entre na máfia com perks especiais</div>
        </div>
        <div>
          <span class="product-price">R$ 30,00</span>
          <button class="buy-btn">Comprar</button>
        </div>
      </div>
    </section>

    <section id="corpos">
      <h2>Corpos Adicionais</h2>
      <div class="product">
        <div>
          <div class="product-name">Corpo Extra - VIP</div>
          <div class="product-desc">Mais slots para personalizar seus personagens</div>
        </div>
        <div>
          <span class="product-price">R$ 15,00</span>
          <button class="buy-btn">Comprar</button>
        </div>
      </div>
      <div class="product">
        <div>
          <div class="product-name">Corpo Extra - Elite</div>
          <div class="product-desc">Slots extras e skins exclusivas</div>
        </div>
        <div>
          <span class="product-price">R$ 25,00</span>
          <button class="buy-btn">Comprar</button>
        </div>
      </div>
    </section>

    <section id="carros">
      <h2>Carros VIP</h2>
      <div class="product">
        <div>
          <div class="product-name">Carro VIP - Esportivo</div>
          <div class="product-desc">Carro esportivo exclusivo para VIPs</div>
        </div>
        <div>
          <span class="product-price">R$ 40,00</span>
          <button class="buy-btn">Comprar</button>
        </div>
      </div>
      <div class="product">
        <div>
          <div class="product-name">Carro VIP - Luxo</div>
          <div class="product-desc">Carro de luxo exclusivo com detalhes personalizados</div>
        </div>
        <div>
          <span class="product-price">R$ 50,00</span>
          <button class="buy-btn">Comprar</button>
        </div>
      </div>
    </section>
  </main>

  <footer>© 2025 Vale Roleplay - Todos os direitos reservados</footer>
</body>
</html>
