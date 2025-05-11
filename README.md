projetos-pessoais/
└── relogio-digital/
    ├── index.html
    ├── style.css
    └── script.js
<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Relógio Digital</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <div class="relogio">
    <h1 id="horas">00:00:00</h1>
  </div>

  <script src="script.js"></script>
</body>
</html>
body {
  background-color: #121212;
  color: #00ffcc;
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
  margin: 0;
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
}

.relogio {
  text-align: center;
  font-size: 3em;
}
function atualizarRelogio() {
  const agora = new Date();
  const horas = agora.getHours().toString().padStart(2, '0');
  const minutos = agora.getMinutes().toString().padStart(2, '0');
  const segundos = agora.getSeconds().toString().padStart(2, '0');

  document.getElementById('horas').textContent = `${horas}:${minutos}:${segundos}`;
}

setInterval(atualizarRelogio, 1000);
atualizarRelogio();
# Relógio Digital 🕒

Um projeto simples de relógio digital feito com HTML, CSS e JavaScript.

## Funcionalidade
- Exibe a hora atual em tempo real
- Interface simples e responsiva

## Como usar
1. Clone o repositório ou baixe os arquivos.
2. Abra o `index.html` em seu navegador.

## Autor
Lucas Barbosa dos Reis
