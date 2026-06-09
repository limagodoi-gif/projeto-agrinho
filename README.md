<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Meu Projeto Responsivo</title>
    <link rel="stylesheet" href="css/style.css">
</head>
<body>

    <header>
        <h1>Agro Quest</h1>
        <p>Uma experiência digital e interativa</p>
    </header>

    <main class="container">
        <section class="card">
            <h2>Bem-vindo ao Projeto</h2>
            <p>Este layout é responsivo, adaptando-se a qualquer tamanho de tela.</p>
            <img src="assets/foto-agro.png" alt="Imagem ilustrativa do projeto" class="img-responsiva">
            
            <button id="botao-interagir">Clique Aqui</button>
        </section>
    </main>

    <script src="js/script.js"></script>
</body>
</html>
/* Configurações Gerais e Cores (Garantindo Contraste) */
body {
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    background-color: #f4f7f6;
    color: #333333;
    margin: 0;
    padding: 0;
}

header {
    background-color: #2e7d32; /* Verde escuro para bom contraste com texto branco */
    color: white;
    text-align: center;
    padding: 2rem;
}

/* Layout Responsivo */
.container {
    max-width: 800px;
    margin: 2rem auto;
    padding: 0 1rem;
}

.card {
    background: white;
    padding: 2rem;
    border-radius: 8px;
    box-shadow: 0 4px 6px rgba(0,0,0,0.1);
}

.img-responsiva {
    max-width: 100%;
    height: auto;
    border-radius: 4px;
    margin-top: 1rem;
}

/* Efeitos Visuais e Interatividade */
button {
    background-color: #2e7d32;
    color: white;
    border: none;
    padding: 0.75rem 1.5rem;
    font-size: 1rem;
    border-radius: 4px;
    cursor: pointer;
    transition: background-color 0.3s ease, transform 0.1s ease;
    margin-top: 1rem;
}

button:hover {
    background-color: #1b5e20; /* Escurece ao passar o mouse */
}
// Aguarda o carregamento do HTML
document.addEventListener("DOMContentLoaded", () => {
    const botao = document.getElementById("botao-interagir");

    // Adiciona interatividade e feedback visual ao usuário
    botao.addEventListener("click", () => {
        alert("Interação realizada com sucesso! O sistema está funcionando de forma fluida.");
    });
});


button:active {
    transform: scale(0.98); /* Efeito de clique sutil */
}
