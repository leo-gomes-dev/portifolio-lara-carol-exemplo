# Descrição do Projeto Final: Portfólio Profissional UI/UX & Web
**Curso:** HTML & CSS Básico  
**Instrutor:** Prof. Leo Gomes Developer  
**Alunas/Docentes:** Lara & Carol  

---

## 1. Visão Geral do Projeto
O objetivo deste projeto final é consolidar os conhecimentos adquiridos em HTML5 e CSS3, unindo a bagagem técnica de desenvolvimento com a expertise que vocês já possuem como **Professoras de Design**. Vocês deverão criar um **Portfólio Profissional** autoral, altamente atraente, com forte apelo visual, tipografia expressiva e micro-interações fluidas.

O grande destaque visual da página será uma **Seção Hero com a imagem em destaque** de cada uma de vocês (ou uma ilustração vetorial que represente sua identidade visual), posicionada estrategicamente para reter a atenção do visitante nos primeiros 3 segundos.

---

## 2. Requisitos Técnicos e de Design
Para garantir nota máxima e um produto final pronto para o mercado, o portfólio deve seguir as seguintes diretrizes:

*   **HTML Semântico:** Uso obrigatório de `<header>`, `<nav>`, `<main>`, `<section>`, `<article>` e `<footer>`.
*   **Seção Hero de Impacto:** Um banner principal com uma foto ou identidade visual marcante, um título forte (H1) e uma chamada para ação (CTA).
*   **Galeria Grid/Flexbox:** Exibição dos melhores projetos de design de vocês utilizando layouts modernos (`display: flex`).
*   **Estética Visual Premium:** Escolha uma paleta de cores harmoniosa, contraste acessível, fontes institucionais modernas (ex: Google Fonts) e efeitos sutis de `transition` ao passar o mouse (hover) nos botões e cards.

---

## 3. Passo a Passo da Execução (Do Início ao Fim)

### Passo 1: Planejamento e Wireframe (O Olhar do Designer)
Antes do código, definam o layout. Desenhem a estrutura no papel ou no Figma:
*   Onde ficará o menu? Como a imagem do Hero se alinhará com o texto de introdução?

### Passo 2: Estruturação do HTML (O Alicerce)
Abram o editor de código (VS Code) e criem o arquivo `index.html`. Criem a estrutura básica e dividam o documento em seções bem claras:
1.  **Header:** Logotipo e Menu de navegação.
2.  **Hero Section:** Sua foto, frase de impacto e botão "Fale Comigo".
3.  **About Section:** Breve biografia destacando sua atuação como professora e designer.
4.  **Portfolio Gallery:** Grid exibindo miniaturas dos seus trabalhos de design.
5.  **Footer:** Direitos autorais e links para redes sociais (LinkedIn, Behance).

### Passo 3: Estilização com CSS (A Magia Visual)
Criem o arquivo `style.css`. Comecem aplicando o "CSS Reset" para remover margens padrões. Em seguida, estilizem:
*   A tipografia global e as cores de fundo.
*   O layout do Hero para que o texto e a imagem fiquem perfeitamente alinhados e responsivos.
*   Efeitos de hover nos botões para torná-los atraentes e clicáveis.

### Passo 4: Revisão e Refinamento
Testem o comportamento dos elementos visuais. Certifiquem-se de que os contrastes estão adequados para leitura e que todos os links funcionam.

---

## 4. Código de Exemplo (Modelo Base)

Abaixo está o modelo funcional separado que serve como ponto de partida para vocês customizarem.

### `index.html`
```html
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Portfólio Profissional | Design & Web</title>
    <link rel="stylesheet" href="style.css">
    <!-- Google Fonts para um design moderno -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@400;600;800&display=swap" rel="stylesheet">
</head>
<body>

    <!-- CABEÇALHO -->
    <header class="navbar">
        <div class="logo">Lara & Carol<span>.design</span></div>
        <nav>
            <ul class="nav-links">
                <li><a href="#inicio">Início</a></li>
                <li><a href="#sobre">Sobre</a></li>
                <li><a href="#portfolio">Portfólio</a></li>
                <li><a href="#contato" class="btn-sm">Contato</a></li>
            </ul>
        </nav>
    </header>

    <main>
        <!-- SEÇÃO HERO (SUA IMAGEM DESTAQUE) -->
        <section id="inicio" class="hero">
            <div class="hero-content">
                <span class="badge">Designer & Professora</span>
                <h1>Criando experiências visuais <span>memoráveis</span>.</h1>
                <p>Especialista em transformar ideias complexas em interfaces atraentes, funcionais e de alto impacto visual.</p>
                <div class="hero-actions">
                    <a href="#portfolio" class="btn btn-primary">Ver Projetos</a>
                    <a href="#contato" class="btn btn-secondary">Vamos Conversar</a>
                </div>
            </div>
            <div class="hero-image-container">
                <!-- Substitua pelo caminho real da sua foto -->
                <img src="https://images.unsplash.com/photo-1573496359142-b8d87734a5a2?q=80&w=600" alt="Sua Imagem Hero" class="hero-img">
                <div class="hero-circle-bg"></div>
            </div>
        </section>

        <!-- SEÇÃO SOBRE -->
        <section id="sobre" class="about">
            <h2>Sobre Mim</h2>
            <p>Atuo na intersecção entre o design estratégico e o desenvolvimento front-end. Como professora de design, minha missão é unir a teoria estética com a prática do código limpo, ensinando e aplicando conceitos que encantam usuários.</p>
        </section>

        <!-- SEÇÃO PORTFÓLIO -->
        <section id="portfolio" class="portfolio">
            <h2>Projetos em Destaque</h2>
            <div class="portfolio-grid">
                <div class="portfolio-card">
                    <div class="card-img-placeholder">UI/UX App Redesign</div>
                    <div class="card-body">
                        <h3>Identidade Visual & App</h3>
                        <p>Estudo de caso completo de interface mobile.</p>
                    </div>
                </div>
                <div class="portfolio-card">
                    <div class="card-img-placeholder">Branding Editorial</div>
                    <div class="card-body">
                        <h3>Design de Marca</h3>
                        <p>Projeto de branding conceitual corporativo.</p>
                    </div>
                </div>
                <div class="portfolio-card">
                    <div class="card-img-placeholder">Web Design Concept</div>
                    <div class="card-body">
                        <h3>Landing Page High-End</h3>
                        <p>Direção de arte e prototipagem responsiva.</p>
                    </div>
                </div>
            </div>
        </section>
    </main>

    <!-- RODAPÉ -->
    <footer id="contato">
        <p>&copy; 2026 Lara & Carol Design. Desenvolvido no curso do Prof. Leo Gomes Developer.</p>
    </footer class="footer">

</body>
</html>
```

### `style.css`
```css
/* RESET PADRÃO */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Plus Jakarta Sans', sans-serif;
}

:root {
    --primary: #6366f1;
    --primary-dark: #4f46e5;
    --dark: #0f172a;
    --light: #f8fafc;
    --text-muted: #64748b;
    --bg-gradient: linear-gradient(135deg, #f5f3ff 0%, #e0e7ff 100%);
}

html {
    scroll-behavior: smooth;
}

body {
    background-color: var(--light);
    color: var(--dark);
    overflow-x: hidden;
}

/* NAVBAR */
.navbar {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 24px 8%;
    background-color: rgba(248, 250, 252, 0.8);
    backdrop-filter: blur(10px);
    position: sticky;
    top: 0;
    z-index: 100;
}

.logo {
    font-size: 1.5rem;
    font-weight: 800;
    color: var(--dark);
}

.logo span {
    color: var(--primary);
}

.nav-links {
    display: flex;
    list-style: none;
    align-items: center;
    gap: 32px;
}

.nav-links a {
    text-decoration: none;
    color: var(--dark);
    font-weight: 600;
    transition: color 0.3s;
}

.nav-links a:hover {
    color: var(--primary);
}

.btn-sm {
    background-color: var(--dark);
    color: #fff !important;
    padding: 10px 20px;
    border-radius: 50px;
}

.btn-sm:hover {
    background-color: var(--primary);
}

/* SEÇÃO HERO */
.hero {
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 60px 8%;
    min-height: 85vh;
    gap: 40px;
}

.hero-content {
    flex: 1;
    max-width: 600px;
}

.badge {
    background-color: rgba(99, 102, 241, 0.1);
    color: var(--primary);
    padding: 6px 16px;
    border-radius: 50px;
    font-weight: 600;
    font-size: 0.85rem;
    display: inline-block;
    margin-bottom: 20px;
}

.hero-content h1 {
    font-size: 3.5rem;
    line-height: 1.1;
    font-weight: 800;
    margin-bottom: 20px;
}

.hero-content h1 span {
    color: var(--primary);
}

.hero-content p {
    font-size: 1.15rem;
    color: var(--text-muted);
    line-height: 1.6;
    margin-bottom: 32px;
}

.hero-actions {
    display: flex;
    gap: 16px;
}

.btn {
    padding: 14px 28px;
    border-radius: 8px;
    text-decoration: none;
    font-weight: 600;
    transition: all 0.3s ease;
}

.btn-primary {
    background-color: var(--primary);
    color: white;
    box-shadow: 0 10px 20px rgba(99, 102, 241, 0.2);
}

.btn-primary:hover {
    background-color: var(--primary-dark);
    transform: translateY(-2px);
}

.btn-secondary {
    border: 2px solid var(--dark);
    color: var(--dark);
}

.btn-secondary:hover {
    background-color: var(--dark);
    color: white;
    transform: translateY(-2px);
}

/* CONTAINER DA IMAGEM HERO */
.hero-image-container {
    flex: 1;
    display: flex;
    justify-content: center;
    position: relative;
}

.hero-img {
    width: 400px;
    height: 400px;
    object-fit: cover;
    border-radius: 30% 70% 70% 30% / 30% 30% 70% 70%; /* Formato orgânico atraente */
    box-shadow: 0 20px 40px rgba(15, 23, 42, 0.15);
    z-index: 2;
    animation: morph 8s ease-in-out infinite alternate;
}

@keyframes morph {
    0% { border-radius: 30% 70% 70% 30% / 30% 30% 70% 70%; }
    100% { border-radius: 50% 50% 30% 70% / 50% 60% 40% 50%; }
}

/* SEÇÃO SOBRE & PORTFÓLIO */
.about, .portfolio {
    padding: 80px 8%;
    text-align: center;
}

.about p {
    max-width: 800px;
    margin: 24px auto 0;
    font-size: 1.2rem;
    line-height: 1.8;
    color: var(--text-muted);
}

.portfolio h2 {
    font-size: 2.5rem;
    margin-bottom: 40px;
}

.portfolio-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
    gap: 32px;
}

.portfolio-card {
    background: #fff;
    border-radius: 16px;
    overflow: hidden;
    box-shadow: 0 10px 30px rgba(0,0,0,0.05);
    transition: transform 0.3s;
    text-align: left;
}

.portfolio-card:hover {
    transform: translateY(-8px);
}

.card-img-placeholder {
    height: 220px;
    background: var(--bg-gradient);
    display: flex;
    align-items: center;
    justify-content: center;
    font-weight: 600;
    color: var(--primary);
}

.card-body {
    padding: 24px;
}

.card-body h3 {
    margin-bottom: 8px;
    font-size: 1.25rem;
}

.card-body p {
    color: var(--text-muted);
}

/* RODAPÉ */
.footer {
    padding: 40px 8%;
    background-color: var(--dark);
    color: rgba(255,255,255,0.7);
    text-align: center;
    margin-top: 60px;
}
```
