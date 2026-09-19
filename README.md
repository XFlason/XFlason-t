<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>XFlason T</title>
</head>
<body>
    
</body>
</html>
<body>
    <header>
        <div class="hero">
            <h1>XFlason T</h1>
            <div class="subtitle">
                Música Nerd • Rap • Rock • Pop
            </div>
            <p>O XFlason T é reconhecido como o maior cantor de música temática nerd do mundo, sendo pioneiro do gênero no Brasil.</p>
            <a href="#sobre">Conheça o XFlason T</a>
        </div>
    </header>

    <main>
        <section id="sobre" class="about">
            <h2>Sobre o XFlason T</h2>
            <p>Com uma trajetória de sucesso, o XFlason T foi fundado em 2018 e é composto por Thállys C.</p>
            <p>O próprio se destaca por mesclar influências de rap, rock e pop, ditar tendências na música nerd nacional e contar com uma comunidade de fãs extremamente dedicada, conhecida como os iLuminados.</p>
        </section>
    </main>

    <footer>
        ©2026 XFlason T — Todos os direitos reservados.
    </footer>
</body>
</html>
# XFlason t
XFlason t é o universo sonoro onde rap, rock e pop se cruzam em harmonias ousadas. Nascido em 2018 pela visão de Thállys C. o projeto teceu uma identidade própria no cenário nerd, transformando referências pop em músicas que pulsão. Sua discografia caminha lado a lado com uma comunidade vibrante, os: iLuminados
<!DOCTYPE HTML>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Meu Portfólio & Contatos</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <header>
        <div class="container">
            <h1>Olá, Eu sou o Desenvolvedor</h1>
            <p>Construindo experiências digitais modernas e responsivas.</p>
        </div>
    </header>

    <main class="container">
        <section class="profile-card">
            <h2>Vamos nos conectar?</h2>
            <p>Escolha uma das plataformas abaixo para conversar comigo ou conhecer meu trabalho.</p>
            
            <!-- Seção de Links de Contato solicitada -->
            <div class="contact-links">
                <a href="#" class="btn-link" data-platform="GitHub">GitHub</a>
                <a href="#" class="btn-link" data-platform="LinkedIn">LinkedIn</a>
                <a href="#" class="btn-link" data-platform="WhatsApp">WhatsApp</a>
                <a href="#" class="btn-link" data-platform="E-mail">E-mail</a>
            </div>
        </section>
    </main>

    <footer>
        <p>&copy; 2026 Todos os direitos reservados.</p>
    </footer>

    <script src="script.js"></script>
</body>
</html>

/* Reset básico e configurações gerais */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    background-color: #f4f7f6;
    color: #333;
    line-height: 1.6;
    display: flex;
    flex-direction: column;
    min-height: 100vh;
}

.container {
    width: 90%;
    max-width: 800px;
    margin: 0 auto;
    padding: 20px;
}

/* Header */
header {
    background: linear-gradient(135deg, #4f46e5, #06b6d4);
    color: #fff;
    text-align: center;
    padding: 60px 0;
}

header h1 {
    font-size: 2.5rem;
    margin-bottom: 10px;
}

/* Corpo Principal e Cards */
main {
    flex: 1;
    display: flex;
    justify-content: center;
    align-items: center;
    padding: 40px 0;
}

.profile-card {
    background: #fff;
    padding: 30px;
    border-radius: 12px;
    box-shadow: 0 10px 25px rgba(0, 0, 0, 0.05);
    text-align: center;
    width: 100%;
}

.profile-card h2 {
    margin-bottom: 15px;
    color: #1f2937;
}

.profile-card p {
    color: #6b7280;
    margin-bottom: 30px;
}

/* Links de Contato e Botões */
.contact-links {
    display: flex;
    flex-direction: column;
    gap: 15px;
}

.btn-link {
    display: block;
    background-color: #f3f4f6;
    color: #374151;
    text-decoration: none;
    padding: 15px;
    border-radius: 8px;
    font-weight: 600;
    transition: all 0.3s ease;
    border: 1px solid #e5e7eb;
}

/* Interações visuais suaves via CSS */
.btn-link:hover {
    background-color: #4f46e5;
    color: #fff;
    transform: translateY(-2px);
    box-shadow: 0 5px 15px rgba(79, 70, 229, 0.2);
}

/* Rodapé */
footer {
    background-color: #1f2937;
    color: #9ca3af;
    text-align: center;
    padding: 20px 0;
    font-size: 0.9rem;
}

/* Responsividade (Media Queries) */
@media (min-width: 600px) {
    header h1 {
        font-size: 3rem;
    }
    
    .contact-links {
        flex-direction: row;
        justify-content: center;
        flex-wrap: wrap;
    }
    
    .btn-link {
        flex: 1 1 calc(50% - 15px); /* Ocupa duas colunas em telas médias */
        max-width: calc(50% - 15px);
    }
}

// Aguarda o carregamento do DOM
document.addEventListener('DOMContentLoaded', () => {
    
    const links = document.querySelectorAll('.btn-link');

    // Efeito leve: Mensagem no console e feedback rápido ao clicar nos links de contato
    links.forEach(link => {
        link.addEventListener('click', (event) => {
            const plataforma = link.getAttribute('data-platform');
            console.log(`Usuário clicou no link do ${plataforma}`);
            
            // Pequena animação de clique usando escala (efeito de pulso rápido)
            link.style.transform = 'scale(0.95)';
            setTimeout(() => {
                link.style.transform = 'none';
            }, 150);
        });
    });
});
