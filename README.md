# -website
Projeto  website
<!DOCTYPE html>
<!DOCTYPE html>
<html>
<head>
  <title>Meu Projeto com Menu</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
    }

    nav {
      background-color: #0077cc;
      padding: 10px;
    }

    nav ul {
      list-style-type: none;
      margin: 0;
      padding: 0;
      display: flex;
    }

    nav ul li {
      margin-right: 20px;
    }

    nav ul li a {
      color: white;
      text-decoration: none;
      font-weight: bold;
    }

    nav ul li a:hover {
      text-decoration: underline;
    }

    main {
      padding: 20px;
    }
  </style>
</head>
<body>

  <nav>
    <ul>
      <li><a href="#sobre">Sobre</a></li>
      <li><a href="#habilidades">Habilidades</a></li>
      <li><a href="#projetos">Projetos</a></li>
      <li><a href="#contato">Contato</a></li>
    </ul>
  </nav>

  <main>
    <h1 id="sobre">Bem-vindo ao Meu Site</h1>
    <p>Informações sobre mim...</p>

    <h2 id="habilidades">Minhas Habilidades</h2>
    <ul>
      <li>HTML</li>
      <li>CSS</li>
      <li>JavaScript</li>
    </ul>

    <h2 id="projetos">Projetos</h2>
    <ol>
      <li>Site Pessoal</li>
      <li>Blog</li>
    </ol>

    <h2 id="contato">Contato</h2>
    <p>Email: sandy@exemplo.com</p>
  </main>

</body>
</html>
<!DOCTYPE html>
<html>
<head>
  <title>Site Responsivo</title>
  <style>
    body {
      margin: 0;
      font-family: Arial, sans-serif;
    }

    nav {
      background-color: #0077cc;
      padding: 10px 20px;
      display: flex;
      justify-content: space-between;
      align-items: center;
    }

    .menu-toggle {
      display: none;
      font-size: 26px;
      color: white;
      cursor: pointer;
    }

    ul.menu {
      list-style: none;
      margin: 0;
      padding: 0;
      display: flex;
    }

    ul.menu li {
      margin-right: 20px;
    }

    ul.menu li a {
      color: white;
      text-decoration: none;
      font-weight: bold;
    }

    ul.menu li a:hover {
      text-decoration: underline;
    }

    @media (max-width: 600px) {
      .menu-toggle {
        display: block;
      }
      ul.menu {
        display: none;
        flex-direction: column;
        background-color: #0077cc;
        margin-top: 10px;
      }
      ul.menu.active {
        display: flex;
      }
      ul.menu li {
        margin: 10px 0;
      }
    }
  </style>
</head>
<body>

  <nav>
    <div class="logo"><strong style="color:white;">Meu Site</strong></div>
    <div class="menu-toggle" onclick="toggleMenu()">☰</div>
    <ul class="menu" id="menu">
      <li><a href="#sobre">Sobre</a></li>
      <li><a href="#habilidades">Habilidades</a></li>
      <li><a href="#projetos">Projetos</a></li>
      <li><a href="#contato">Contato</a></li>
    </ul>
  </nav>

  <main style="padding: 20px;">
    <h1 id="sobre">Sobre Mim</h1>
    <p>Informações sobre Sandy e o desafio de projeto.</p>

    <h2 id="habilidades">Habilidades</h2>
    <ul>
      <li>HTML</li>
      <li>CSS</li>
      <li>JavaScript</li>
    </ul>

    <h2 id="projetos">Projetos</h2>
    <ol>
      <li>Site Pessoal</li>
      <li>Blog</li>
    </ol>

    <h2 id="contato">Contato</h2>
    <p>Email: sandy@exemplo.com</p>
  </main>

  <script>
    function toggleMenu() {
      var menu = document.getElementById("menu");
      menu.classList.toggle("active");
    }
  </script>

</body>
</html>
