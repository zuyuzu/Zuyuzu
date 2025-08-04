## Hi there 👋

<!--
**zuyuzu/Zuyuzu** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
<!DOCTYPE html><html lang="pt-BR">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Galeria de Design</title>
  <style>
    body {
      font-family: sans-serif;
      margin: 0;
      padding: 2rem;
      background-color: #f7f7f7;
    }
    h1 {
      text-align: center;
      margin-bottom: 2rem;
    }
    .filters {
      text-align: center;
      margin-bottom: 2rem;
    }
    .filters button {
      margin: 0 0.5rem;
      padding: 0.5rem 1rem;
      cursor: pointer;
      border: none;
      border-radius: 5px;
      background-color: #ddd;
    }
    .filters button.active {
      background-color: #333;
      color: white;
    }
    .gallery {
      display: grid;
      grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
      gap: 1rem;
    }
    .item {
      background-color: white;
      border-radius: 10px;
      overflow: hidden;
      box-shadow: 0 2px 8px rgba(0,0,0,0.1);
      transition: transform 0.3s ease;
    }
    .item:hover {
      transform: scale(1.02);
    }
    .item img {
      width: 100%;
      display: block;
    }
    .lightbox {
      display: none;
      position: fixed;
      top: 0; left: 0; right: 0; bottom: 0;
      background: rgba(0,0,0,0.8);
      justify-content: center;
      align-items: center;
    }
    .lightbox img {
      max-width: 90%;
      max-height: 90%;
    }
  </style>
</head>
<body>
  <h1>Galeria de Design</h1>
  <div class="filters">
    <button class="active" onclick="filterItems('all')">Todos</button>
    <button onclick="filterItems('poster')">Pôsteres</button>
    <button onclick="filterItems('cartaz')">Cartazes</button>
    <button onclick="filterItems('convite')">Convites</button>
    <button onclick="filterItems('marca')">Marcas</button>
    <button onclick="filterItems('modelo')">Modelos</button>
  </div>
  <div class="gallery">
    <div class="item poster"><img src="https://via.placeholder.com/400x500?text=Poster+1" alt="Poster"></div>
    <div class="item cartaz"><img src="https://via.placeholder.com/400x500?text=Cartaz+1" alt="Cartaz"></div>
    <div class="item convite"><img src="https://via.placeholder.com/400x500?text=Convite+1" alt="Convite"></div>
    <div class="item marca"><img src="https://via.placeholder.com/400x500?text=Marca+1" alt="Marca"></div>
    <div class="item modelo"><img src="https://via.placeholder.com/400x500?text=Modelo+1" alt="Modelo"></div>
    <div class="item poster"><img src="https://via.placeholder.com/400x500?text=Poster+2" alt="Poster"></div>
    <div class="item cartaz"><img src="https://via.placeholder.com/400x500?
