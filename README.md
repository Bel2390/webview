# webview
Projeto pessoal- Página de E-commerce
<!DOCTYPE html>
<html lang="pt-br">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Electronic's Paradise</title>
  <link rel="stylesheet" href="styles.css">
</head>
   
<body>
  <!-- Cabeçalho -->
  <header>
    <nav class="Inicio">
      <h1>Electronic's Paradise</h1>
      <ul>
        <li><a href="#home"  id="our-products-link">Our products</a></li>
        <li><a  id="reviews-link"  href="#products">Reviews</a></li>
        <li><a id="contact-link"  href="#contact">Contact</a></li>
       
      </ul>
      <!-- Ícone do Carrinho -->
      <a href="#" class="cart-icon">
      
       <span id="cart-count">0</span>
  
        <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="currentColor" class="bi bi-cart" viewBox="0 0 16 16">
          <path d="M0 1.5A.5.5 0 0 1 .5 1h1a.5.5 0 0 1 .485.379L2.89 5H14.5a.5.5 0 0 1 .491.592l-1.5 8A.5.5 0 0 1 13 14H4a.5.5 0 0 1-.491-.408L1.01 2H.5a.5.5 0 0 1-.5-.5zm3.14 4L4.89 13H13l1.25-6.5H3.14z" />
          <path d="M4.5 16a1.5 1.5 0 1 1 0-3 1.5 1.5 0 0 1 0 3zm7 0a1.5 1.5 0 1 1 0-3 1.5 1.5 0 0 1 0 3z" />
        </svg>
     
      </a>
        <div id="cart-box" class="hidden">
  <h3>Your Cart</h3>
  <ul id="cart-items"></ul>
  <button id="checkout-btn">Check-out</button>
</div>
    </nav>
     <div id="contact-tab" class="hidden">(XXX) 555-xxxx</div>
      <div class="header-content">
    <h3>Here, your experience matters</h3>
    <img src="https://images.pexels.com/photos/2569997/pexels-photo-2569997.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1" alt="Imagem do Header">
  </div>
      </header>

  

  <!-- Conteúdo Principal -->
  <main>
    <div class="promo-content">
      
      <div class="promo-container">
    <img src="https://cdn.pixabay.com/photo/2020/08/26/14/29/smartphone-5519654_1280.jpg" alt="propaganda" class="add-img">
    <div class="promo-box">
      <h2>Special promotion available now! <br> Don't miss out!</h2>
       <p>Buy one tablet and get another with earphones for  half  price!</p>
    </div>
  </div>
    
      <button class="add-to-cart-btn" data-product-id="1">Buy now</button>
    </div>
 <div class="headphone-container" id="headphone-container">
   <div class="an-box">
     <p>$99</p>
  <h4>Our very best headphone!</h4>
   
  <img src="https://cdn.pixabay.com/photo/2019/08/27/13/35/headphones-4434215_1280.jpg" alt="phone" class="headphone" id="phone-photo">
     
</div>
  
   <button class="add-to-cart-btn"  data-product-id="1">Add to cart</button>
    </div>
    <div id="computer-container"  class="computer-container">
      <div class="prop-box">
        <p> $500</p>
        <h5>Get our powerful computer</h5>
    <img src="https://cdn.pixabay.com/photo/2020/10/21/18/07/laptop-5673901_1280.jpg" alt="comp" class="prop-two" id="comp-photo">
      
      </div>
      <button  class="add-to-cart-btn" data-product-id="2"> Add to cart</button>
    </div>
    <div class="review-container">
      <h6>Reviews⭐⭐⭐⭐⭐</h6>
  <div class="review-box">
   
    <h7>Anonymous costumer<br>⭐⭐⭐⭐⭐</h7>
    <p>Overall, a nice experience. Great product, delivery was fast, no complaints at all.</p>
  </div>
  <div class="review-box">
    <h7>Michaela<br>⭐⭐⭐⭐</h7>
    <p>Good quality, but the delivery took a bit longer than expected.</p>
  </div>
</div>
        
  </main>
</body>
</html>

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

/* Header fixo */

 header {
  
   position: static;
  top: 0;
  left: 0;
  width: 100%;
  background-color: #010101;
  z-index: 1000;
}


.Inicio {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 0 2rem;
  height: 4rem;
  max-width: 1200px;
  margin: 0 auto;
}

.Inicio h1 {
  color: #31a4c8;
  font-size: 1.5rem;
  font-family: Optima, sans-serif;
}

.Inicio ul {
  list-style: none;
  display: flex;
  gap: 2rem;
}

.Inicio ul li a {
  text-decoration: none;
  color: #31a4c8;
  font-size: 1rem;
  font-weight: bold;
  transition: color 0.3s ease;
}

.Inicio ul li a:hover {
  color: #007bff;
}

/* Ícone do Carrinho */
.cart-icon svg {
  fill: #31a4c8;
  transition: fill 0.3s ease;
}

.cart-icon:hover svg {
  fill: #007bff;
}



/* Conteúdo Principal */
body {
  font-family: Arial, sans-serif;
  background-color: #f2f5f7;
}

main {
  margin-top: 2rem;
  padding: 2rem;
  text-align: center;
}



.promo-content button {
    background-color: red;
  color: white;
  padding: 1rem 2rem; /* Aumenta o tamanho do botão */
  border: none;
  border-radius: 8px; /* Cantos mais arredondados */
  font-size: 1.25rem; /* Tamanho maior do texto */
  font-weight: bold; /* Deixa o texto em negrito */
  cursor: pointer;
  transition: background-color 0.3s ease;
  position: relative;
  bottom: 100px;
  left: 550px;
  min-width: 200px; /* Largura mínima para uniformidade */
  display: flex; /* Utiliza flexbox */
  justify-content: center; /* Centraliza horizontalmente */
  align-items: center; /* Centraliza verticalmente */
  text-align: center; /* Garante alinhamento do texto */
}

.promo-content button:hover {
  background-color: darkred;
}

.add-img{
  width:400px;
  height:300px;
  position:absolute
}


.promo-container {
   display: flex; /* Alinha os filhos horizontalmente */
  align-items: center; /* Centraliza verticalmente */
  gap: 1rem; /* Espaço entre a imagem e o retângulo */
  margin-top: 2rem; /* Espaçamento entre promo-container e header */
  position: relative; /* Garante que siga o fluxo normal */
}

/* Estilo do retângulo */
.promo-box {
  background-color: #c8a2c8
    ; /* Cinza claro */
  padding: 1rem; /* Espaçamento interno */
  border-radius: 8px; /* Cantos arredondados */
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1); /* Sombra leve */
  width: 500px; /* Largura máxima */
  height: 300px; /* Altura fixa */
  font-family: Arial, sans-serif;
  color: #333; /* Texto escuro */
  position:relative;
  left:400px
  
    }
h2{
  color:black;
  position:relative;
  font-family: "Cinzel", serif;
  font-optical-sizing: auto;
  font-weight: <weight>;
  right:20px
}
p{
  position:relative;
  top:60px;
  left:0px
}
.header-content {
  display: flex; /* Posiciona os filhos lado a lado */
  align-items: center; /* Centraliza verticalmente */
  justify-content: space-between; /* Ajusta a distribuição */
  gap: 1rem; /* Espaçamento entre o h3 e a imagem */
  padding: 1rem 2rem; /* Espaçamento interno opcional */
}
.header-content h3 {
  font-size: 2rem;
  color: grey;
  font-family: fantasy, Copperplate;
  margin: 0;
  position:relative;
  left:100px
}
.header-content img {
  width: 60%; /* Ajuste conforme o tamanho desejado */
  height: auto;
  object-fit: cover;
  border-radius: 8px; /* Opcional: cantos arredondados 
  */
  
}

   .headphone-container {
    position: relative; /* Define o contexto para posicionamento absoluto */
  align-items: center;
  justify-content: center;
  gap: 1rem;
  margin-top: 3rem;
  padding: 2rem; /* Espaçamento interno */
}

.headphone {
 position:relative;
  left:100px;
   width: 250px;
  height: 200px;
  object-fit: cover;
  border-radius: 8px; 
}

.an-box{
    position: relative; /* Define o contexto para elementos internos */
  background-color: #d3d3d3;
  padding: 5rem;
  border-radius: 8px;
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
  width: 500px;
  height: 300px;
  z-index: 1; /* Certifique-se de que isso seja menor que o botão */
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  overflow: visible; /* Evita que conteúdo ultrapasse os limites */
  margin: auto;}

.an-box h4 {
     margin-bottom: 1rem; /* Espaçamento em relação à imagem */
  font-family: "Cinzel", serif;
  font-size: 1.5rem;
  color: #333;
  text-align: center;
}
.headphone-container button {
    position: absolute; /* Posiciona o botão em relação ao .headphone-container */
  z-index: 2; /* Garante que o botão ficará sobre o .an-box */
  bottom: 100px; /* Posiciona o botão sobre o retângulo */
  right: 47%; /* Centraliza horizontalmente no contêiner */
  transform: translateX(-50%); /* Ajusta a posição central */
  background-color: red;
  color: white;
  width: 150px; /* Define uma largura fixa */
  height: 50px; /* Define uma altura fixa */
  border: none;
  border-radius: 8px;
  font-size: 1rem; /* Ajuste o tamanho da fonte */
  font-weight: bold;
  text-align: center;
  line-height: 50px; /* Centraliza verticalmente o texto dentro do botão */
  cursor: pointer;
  transition: background-color 0.3s ease;
margin-top:1rem
}

.headphone-container button:hover {
  background-color: darkred;
}   
.an-box p{
  position: absolute; /* Torna o parágrafo posicionado em relação ao contêiner pai */
    z-index: 2; /* Garante que ele fique sobre outros elementos */
    top: 50%; /* Centraliza verticalmente no contêiner */
    left:25%; /* Centraliza horizontalmente no contêiner */
    transform: translate(-50%, -50%); /* Ajusta para o centro exato */
    font-size: 1.5rem; /* Ajuste o tamanho da fonte */
    color: black; /* Ajuste a cor do texto conforme o design */
    text-align: center; /* Centraliza o texto */
    margin: 0; /* Remove margens padrão */
    padding: 0; /* Remove espaçamento extra */
    font-weight: bold; /* Torna o texto mais destacado */
}
.prop-two{
  width:250px;
    object-fit: cover;
  border-radius: 8px; 
  position:relative;
  left:65px; 
}

.prop-box{
  position: relative; /* Necessário para que o botão seja posicionado em relação ao retângulo */
  background-color: #d3d3d3;
  padding: 5rem;
  border-radius: 8px;
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
  width: 500px;
  height: 300px;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  overflow: visible; /* Evita cortes do conteúdo interno */
  margin: auto;
}

.computer-container button{
  position: absolute; /* Posiciona o botão em relação ao .prop-box */
  z-index: 2; /* Garante que o botão fique sobre o .prop-box */
  bottom: 100px; /* Ajusta a distância da base do retângulo */
  right: 50%; /* Centraliza horizontalmente no .prop-box */
  transform: translateX(-50%); /* Garante alinhamento central */
  background-color: red;
  color: white;
  width: 150px;
  height: 50px;
  border: none;
  border-radius: 8px;
  font-size: 1rem;
  font-weight: bold;
  text-align: center;
  line-height: 50px;
  cursor: pointer;
  transition: background-color 0.3s ease;
}

.computer-container{
 position: relative; /* Garante que o botão seja posicionado em relação a este contêiner */
  display: flex;
  flex-direction: column; /* Alinha os elementos verticalmente */
  align-items: center; /* Centraliza os filhos horizontalmente */
  justify-content: center;
  gap: 1rem;
  margin-top: 3rem;
  padding: 2rem; /* Espaçamento interno */
}
.computer-container button:hover {
  background-color: darkred;
}
.prop-box p{
  position:absolute;
  top:120px;
  left:70px;
  font-size: 1.5rem;
  font-color:black;
  font-weight:bold
}
.prop-box h5{
  position:absolute;
  top:20px;
 
  font-size: 1.2rem;
   font-family: "Cinzel", serif;
  font-size: 1.5rem;
  color: #333;
}

.review-container{  
  display: flex; /* Posiciona os elementos lado a lado */
  flex-wrap: wrap; /* Permite quebra de linha se necessário */
  justify-content: center; /* Centraliza horizontalmente */
  align-items: flex-start; /* Alinha os elementos no topo */
  gap: 1rem; /* Espaçamento entre os boxes */
  margin-top: 2rem; /* Espaçamento superior */
  padding: 1rem; /* Espaçamento interno */
}

.review-container h6{
    width: 100%; /* Faz o título ocupar toda a largura do container */
  text-align: center; /* Centraliza o texto */
  margin-bottom: 1rem; /* Adiciona espaço abaixo do título */
  font-size: 1.6rem;
  font-family: "Cinzel", serif;
  color: #333;
}


.review-box h7{
  font-weight: bold;
  font-size: 1.2rem;
  margin-bottom: 0.5rem; /* Espaço entre o nome e o comentário */
}
.review-box p{
    font-size: 1rem;
  color: #333;
  position: relative; /* Permite movimentar o elemento */
  top: 5px; /* Ajuste vertical */
  left: 10px; /* Ajuste horizontal */
  word-wrap: break-word;
}

.review-box, .review-box-two {
   flex: 0 0 300px; /* Define uma largura fixa para as caixas */
  max-width: 300px; /* Garante que o tamanho não ultrapasse 300px */
  background-color: #fff;
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
 
  padding: 1rem;
  text-align: left; /* Ajusta alinhamento do texto */
  display: flex;
  flex-direction: column; /* Alinha itens verticalmente */
  gap: 0.5rem; /* Espaçamento interno entre os elementos */
}
#contact-tab {
  position: absolute;
  top: 50px; /* Alinhe a aba com o botão "Contact" */
  right: 100px; /* Ajuste conforme necessário para alinhar à esquerda do botão */
  padding: 10px;
  width: 200px; /* Largura da aba */
  background-color:black;
  border: 1px solid rgba(204, 204, 204, 0.7); /* Borda com transparência */
  border-radius: 5px;
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
  transform: scaleY(0); /* Altura inicial da aba (colapsada) */
  transform-origin: top; /* Origem da transformação no topo */
  transition: transform 0.3s ease-in-out; /* Transição suave */
  z-index: 1000;
  font-size: 14px;
  overflow: hidden;
  display: none; /* Aba fica oculta inicialmente */
color:white;
}

/* Classe para exibir a aba */
#contact-tab.show {
  display: block; /* Torna visível */
  transform: scaleY(1); /* Expande verticalmente */
}
.cart-icon {
  position: relative;
  display: inline-flex;
  align-items: center;
}

#cart-count {
  background-color: red;
  color: white;
  font-size: 0.8rem;
  font-weight: bold;
  border-radius: 50%;
  width: 20px;
  height: 20px;
  display: flex;
  justify-content: center;
  align-items: center;
  position: absolute;
  top: -10px;
  right: -10px;
}


#cart-items {
  list-style: none;
  padding: 0;
  margin: 0;
  max-height: 200px;
  overflow-y: auto; /* Permite rolagem caso necessário */
}

#cart-items li {
  display: flex;
  align-items: center;
  margin-bottom: 1rem;
}

#cart-items img {
  width: 50px;
  height: 50px;
  object-fit: cover;
  margin-right: 1rem;
}

#checkout-btn {
  width: 100%;
  background-color: red;
  color: white;
  border: none;
  border-radius: 8px;
  padding: 0.5rem;
  cursor: pointer;
  font-size: 1rem;
}

#checkout-btn:hover {
  background-color: darkred;
}
#cart-box {
  display: none; /* Oculta inicialmente */
  position: absolute;
  top: 50px; /* Ajuste conforme necessário */
  right: 0;
  width: auto; /* Largura do carrinho */
  background-color: white;
  border: 1px solid #ccc;
  border-radius: 8px;
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
  z-index: 1000;
  padding:6rem;
  opacity: 0;
  transition: opacity 0.3s ease, display 0s ease 0.3s;
}
#cart-box.hidden {
  display: none;
  opacity: 0;
}
#cart-box.visible {
 display: block;
  opacity: 1;
  transition: opacity 0.3s ease;
}

document.getElementById("our-products-link").addEventListener("click", function (event) {
    event.preventDefault(); // Previne o comportamento padrão do link

    // Seleciona os containers que devem ser mostrados
    const headphoneContainer = document.querySelector(".headphone-container");
    const computerContainer = document.querySelector(".computer-container");

    // Faz scroll para o primeiro elemento
    headphoneContainer.scrollIntoView({ behavior: "smooth" });

    // Aguarda o scroll do primeiro elemento antes de ir para o segundo
    setTimeout(() => {
      computerContainer.scrollIntoView({ behavior: "smooth" });
    }, 1000); // Ajuste o tempo conforme necessário
  });
// Capturar o elemento do link "Reviews"
const reviewsLink = document.getElementById("reviews-link");

// Capturar o container de reviews
const reviewContainer = document.querySelector(".review-container");

// Adicionar o evento de clique ao link
reviewsLink.addEventListener("click", (event) => {
  // Prevenir o comportamento padrão do link
  event.preventDefault();

  // Rolagem suave até a seção de reviews
  reviewContainer.scrollIntoView({ behavior: "smooth" });
});
// Capturar o link "Contact" e a aba
const contactLink = document.getElementById("contact-link");
const contactTab = document.getElementById("contact-tab");

// Alternar visibilidade da aba ao clicar no botão "Contact"
contactLink.addEventListener("click", (event) => {
  event.preventDefault(); // Prevenir comportamento padrão do link

  // Alternar a classe 'show' para controlar a exibição
  if (contactTab.classList.contains("show")) {
    contactTab.classList.remove("show");
    setTimeout(() => {
      contactTab.style.display = "none";
    }, 300); // Tempo deve coincidir com o tempo da transição no CSS
  } else {
    contactTab.style.display = "block";
    setTimeout(() => {
      contactTab.classList.add("show");
    }, 10); // Pequeno delay para aplicar a transição
  }
});

// Variável para armazenar o número de itens no carrinho
let cartItemCount = 0;

// Função para atualizar o contador do carrinho
function updateCartCount() {
  const cartCountElement = document.getElementById("cart-count");
  cartCountElement.textContent = cartItemCount;
}

// Função para adicionar item ao carrinho
function addToCart(itemName) {
  cartItemCount++; // Incrementa o número de itens
  updateCartCount(); // Atualiza o contador no cabeçalho

  // Opcional: Exibir uma mensagem temporária
  alert(`${itemName} foi adicionado ao carrinho!`);
}

// Capturar os botões de "Add to cart"
const computerButton = document.querySelector(".computer-container button");
const headphoneButton = document.querySelector(".headphone-container button");

// Adicionar eventos de clique aos botões
computerButton.addEventListener("click", () => addToCart("Computador"));
headphoneButton.addEventListener("click", () => addToCart("Headphone"));

 
const cartIcon = document.querySelector(".cart-icon");
const cartBox = document.getElementById("cart-box");

cartIcon.addEventListener("click", () => {
  if (cartBox.classList.contains("hidden")) {
    cartBox.classList.remove("hidden");
    cartBox.classList.add("visible");
  } else {
    cartBox.classList.remove("visible");
    cartBox.classList.add("hidden");
  }
});

document.addEventListener("DOMContentLoaded", () => {
  const cartIcon = document.querySelector(".cart-icon");
  const cartBox = document.getElementById("cart-box");
  const cartItems = document.getElementById("cart-items");
  const cartCount = document.getElementById("cart-count");
  const checkoutBtn = document.getElementById("checkout-btn");

  let cart = {}; // Agora é um objeto para armazenar a quantidade de cada produto

  // Simulação de produtos
  const products = {
    1: { name: "Headphones", image: "https://cdn.pixabay.com/photo/2019/08/27/13/35/headphones-4434215_1280.jpg", price: 100 },
    2: { name: "Computer", image: "https://cdn.pixabay.com/photo/2020/10/21/18/07/laptop-5673901_1280.jpg", price: 1500 }
  };

  // Função para adicionar produto ao carrinho
  function addToCart(productId) {
    const product = products[productId];
    if (product) {
      if (!cart[productId]) {
        cart[productId] = { ...product, quantity: 1 }; // Se o produto não está no carrinho, adiciona com quantidade 1
      } else {
        cart[productId].quantity++; // Se o produto já está no carrinho, aumenta a quantidade
      }
      updateCart();
    }
  }

  // Atualiza a UI do carrinho
  function updateCart() {
    // Atualiza o contador de itens no carrinho
    let totalItems = 0;
    Object.keys(cart).forEach((productId) => {
      totalItems += cart[productId].quantity; // Soma a quantidade de cada produto
    });
    cartCount.textContent = totalItems;

    // Limpa os itens do carrinho
    cartItems.innerHTML = "";

    // Adiciona os itens ao carrinho
    Object.keys(cart).forEach((productId) => {
      const item = cart[productId];
      const li = document.createElement("li");
      li.innerHTML = `
        <img src="${item.image}" alt="${item.name}">
        <span>${item.name}</span> - Quantidade: ${item.quantity}
        <button class="remove-btn" data-id="${productId}">Remove</button>
      `;
      cartItems.appendChild(li);
    });

    // Atualiza os botões de remoção
    document.querySelectorAll(".remove-btn").forEach((button) => {
      button.addEventListener("click", (e) => {
        const productId = e.target.dataset.id;
        delete cart[productId]; // Remove o produto do carrinho
        updateCart();
      });
    });
  }

  // Adicionar eventos de clique aos botões "Add to cart"
  document.querySelectorAll(".add-to-cart-btn").forEach((button) => {
    button.addEventListener("click", (e) => {
      const productId = parseInt(e.target.dataset.productId, 10);
      addToCart(productId);
    });
  });

  

  // Ação do botão "Check-out"
  checkoutBtn.addEventListener("click", () => {
    alert("Proceeding to checkout...");
    cart = {}; // Limpa o carrinho
    updateCart();
  });
});
