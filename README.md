<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Portal Flash News: Notícias atualizadas diariamente sobre tecnologia, saúde, política, esportes e muito mais. Mantenha-se informado.">
    <meta name="keywords" content="notícias, últimas notícias, tecnologia, saúde, política, esportes, Brasil, mundo, jornal, online, flash news">
    <meta name="author" content="Portal Flash News">
    <meta name="robots" content="index, follow"> <title>Portal Flash News - Últimas Notícias do Dia</title>
    
    <link href="https://fonts.googleapis.com/css2?family=Merriweather:wght@700&family=Open+Sans:wght@400;600;700&display=swap" rel="stylesheet">
    
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
    
    <style>
        /* Estilos Personalizados */
        body { 
            font-family: 'Open Sans', sans-serif; 
            background-color: #f0f2f5; /* Um cinza mais suave */
            color: #333;
        }
        .navbar-brand { 
            font-family: 'Merriweather', serif;
            font-weight: 700; 
            font-size: 1.8rem;
            color: #007bff !important; /* Cor primária do Bootstrap */
        }
        .navbar-nav .nav-link {
            font-weight: 600;
            color: rgba(255, 255, 255, 0.75);
            transition: color 0.3s ease;
        }
        .navbar-nav .nav-link:hover {
            color: #fff;
        }
        .hero-section {
            background-color: #e9ecef;
            padding: 50px 0;
            text-align: center;
            border-bottom: 1px solid #dee2e6;
            margin-bottom: 30px;
        }
        .hero-section h1 {
            font-family: 'Merriweather', serif;
            font-weight: 700;
            color: #212529;
            margin-bottom: 15px;
        }
        .article-card { 
            transition: transform 0.2s ease-in-out, box-shadow 0.2s; 
            border: none;
            border-radius: .5rem;
            overflow: hidden;
        }
        .article-card:hover { 
            transform: translateY(-5px); 
            box-shadow: 0 8px 30px rgba(0,0,0,0.1); 
        }
        .article-card img {
            height: 200px; /* Altura fixa para as imagens dos cards */
            object-fit: cover; /* Garante que a imagem preencha o espaço sem distorcer */
            width: 100%;
        }
        .article-card .card-body {
            padding: 20px;
        }
        .article-card .card-title {
            font-family: 'Merriweather', serif;
            font-size: 1.35rem;
            margin-bottom: 10px;
        }
        .article-card .card-text {
            font-size: 0.95rem;
            color: #6c757d;
        }
        .ad-space { 
            background-color: #e2e6ea; 
            padding: 25px; 
            text-align: center; 
            border: 1px dashed #adb5bd; 
            margin-bottom: 20px;
            color: #495057;
            font-size: 0.9rem;
            min-height: 250px; /* Altura mínima para banners retangulares */
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
        }
        .ad-space.ad-horizontal {
            min-height: 90px; /* Altura mínima para banners horizontais */
            width: 100%;
        }
        .sidebar .list-group-item {
            border: none;
            border-bottom: 1px solid #eee;
            padding-left: 0;
        }
        .sidebar .list-group-item:last-child {
            border-bottom: none;
        }
        .footer {
            background-color: #212529;
            color: #f8f9fa;
            padding: 40px 0;
            margin-top: 50px;
        }
        .footer a {
            color: #007bff;
            text-decoration: none;
            transition: color 0.2s;
        }
        .footer a:hover {
            color: #fff;
        }

        /* Cookie Consent Banner */
        #cookieConsent {
            display: none; /* Escondido por padrão */
            position: fixed;
            bottom: 0;
            left: 0;
            width: 100%;
            background-color: rgba(0, 0, 0, 0.85);
            color: white;
            padding: 15px 20px;
            text-align: center;
            box-shadow: 0 -2px 10px rgba(0,0,0,0.2);
            z-index: 1000;
            font-size: 0.9em;
        }
        #cookieConsent button {
            background-color: #007bff;
            color: white;
            border: none;
            padding: 8px 15px;
            border-radius: 5px;
            cursor: pointer;
            margin-left: 15px;
            transition: background-color 0.3s ease;
        }
        #cookieConsent button:hover {
            background-color: #0056b3;
        }
    </style>
</head>
<body>

    <nav class="navbar navbar-expand-lg navbar-dark bg-dark sticky-top">
        <div class="container">
            <a class="navbar-brand" href="#">Flash News</a>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarNav">
                <ul class="navbar-nav me-auto mb-2 mb-lg-0">
                    <li class="nav-item"><a class="nav-link active" aria-current="page" href="#">Início</a></li>
                    <li class="nav-item"><a class="nav-link" href="#">Política</a></li>
                    <li class="nav-item"><a class="nav-link" href="#">Economia</a></li>
                    <li class="nav-item"><a class="nav-link" href="#">Esportes</a></li>
                    <li class="nav-item"><a class="nav-link" href="#">Tecnologia</a></li>
                    <li class="nav-item"><a class="nav-link" href="#">Saúde</a></li>
                    <li class="nav-item"><a class="nav-link" href="#">Entretenimento</a></li>
                </ul>
                <form class="d-flex" role="search">
                    <input class="form-control me-2" type="search" placeholder="Buscar Notícias..." aria-label="Search">
                    <button class="btn btn-outline-light" type="submit">Buscar</button>
                </form>
            </div>
        </div>
    </nav>

    <div class="hero-section">
        <div class="container">
            <h1>Manchete Principal: Brasil Alcança Recorde em Exportações Agrícolas!</h1>
            <p class="lead">Novos acordos comerciais impulsionam o agronegócio, gerando milhões de empregos e fortalecendo a balança comercial do país.</p>
            <a href="article-page-example.html" class="btn btn-primary btn-lg">Leia a Notícia Completa</a>
            
            <div class="ad-space ad-horizontal mx-auto mt-4" style="max-width: 970px;">
                <p>ESPAÇO PARA ANÚNCIO (970x90 ou 728x90) - Destaque Principal</p>
                <p><small>(Google AdSense ou Venda Direta)</small></p>
                </div>
        </div>
    </div>

    <div class="container mt-4">
        <div class="row">

            <div class="col-lg-8">
                <h2 class="mb-4 text-dark">Últimas Notícias</h2>

                <div class="ad-space ad-horizontal mb-4">
                    <p>ESPAÇO PARA ANÚNCIO (728x90) - Acima das Notícias</p>
                    <p><small>(Google AdSense ou Rede de Anúncios)</small></p>
                    </div>

                <div class="card mb-4 article-card">
                    <img src="https://via.placeholder.com/800x400/007bff/fff?text=Saude+Publica" class="card-img-top" alt="Imagem Notícia Saúde">
                    <div class="card-body">
                        <h5 class="card-title">Avanço na Saúde Pública: Novo Programa Nacional é Lançado</h5>
                        <p class="card-text">O Ministério da Saúde anunciou um novo programa que visa ampliar o acesso a exames gratuitos em todo o país. A iniciativa, que visa reduzir filas e melhorar o diagnóstico precoce, começa a valer no próximo mês e abrangerá diversas especialidades. Detalhes sobre o agendamento e locais de atendimento serão divulgados em breve. Especialistas veem a medida como um passo crucial para a democratização da saúde.</p>
                        <a href="article-page-example.html" class="btn btn-primary">Leia Mais</a>
                    </div>
                </div>

                <div class="card mb-4 article-card">
                    <img src="https://via.placeholder.com/800x400/28a745/fff?text=Tecnologia+5G" class="card-img-top" alt="Imagem Notícia Tecnologia">
                    <div class="card-body">
                        <h5 class="card-title">Tecnologia 5G se Expande Rapidamente pelo Brasil</h5>
                        <p class="card-text">As principais operadoras já iniciaram a instalação de antenas em cidades de médio porte, prometendo internet móvel até 10x mais rápida que o 4G. A expansão do 5G promete revolucionar diversos setores, desde a telemedicina até a indústria 4.0, abrindo novas fronteiras para a conectividade e inovação no país. Saiba quais cidades já estão recebendo a nova tecnologia e os impactos esperados.</p>
                        <a href="article-page-example.html" class="btn btn-primary">Leia Mais</a>
                    </div>
                </div>

                <div class="card mb-4 article-card">
                    <img src="https://via.placeholder.com/800x400/ffc107/333?text=Futebol+Feminino" class="card-img-top" alt="Imagem Notícia Esportes">
                    <div class="card-body">
                        <h5 class="card-title">Esportes: Seleção Brasileira Feminina Vence Amistoso Internacional com Goleada</h5>
                        <p class="card-text">A seleção feminina de futebol venceu por 3 a 1 em um amistoso disputado em solo europeu contra a atual campeã mundial, demonstrando grande preparo técnico e físico para os próximos desafios. Com atuações de destaque de Marta e Debinha, o time brasileiro mostrou um futebol envolvente e ofensivo, animando os torcedores para a próxima Copa. Analisamos os lances e o desempenho das atletas.</p>
                        <a href="article-page-example.html" class="btn btn-primary">Leia Mais</a>
                    </div>
                </div>

                <div class="card mb-4 article-card">
                    <img src="https://via.placeholder.com/800x400/6f42c1/fff?text=Economia+Mercado" class="card-img-top" alt="Imagem Notícia Economia">
                    <div class="card-body">
                        <h5 class="card-title">Mercado Financeiro: Bolsa de Valores Reage Positivamente a Novas Medidas Econômicas</h5>
                        <p class="card-text">Após o anúncio do pacote de estímulos, o mercado de ações teve um dia de forte alta, com investidores reagindo com otimismo às perspectivas de recuperação econômica. Analistas apontam que a confiança do mercado pode ser um catalisador para novos investimentos. Detalhes sobre os setores que mais se beneficiaram e as expectativas para os próximos meses.</p>
                        <a href="article-page-example.html" class="btn btn-primary">Leia Mais</a>
                    </div>
                </div>

            </div>

            <div class="col-lg-4">
                <div class="ad-space mb-4" style="height: 300px;">
                    <p>ESPAÇO PARA ANÚNCIO (300x250/300) - Sidebar Superior</p>
                    <p><small>(Google AdSense - Bloco de Anúncios Responsivo)</small></p>
                    </div>

                <div class="card mb-4 shadow-sm">
                    <div class="card-body">
                        <h5 class="card-title text-dark">Notícias Populares</h5>
                        <ul class="list-group list-group-flush">
                            <li class="list-group-item"><a href="#" class="text-dark fw-bold">1. Inteligência Artificial: Os dilemas éticos da nova era.</a></li>
                            <li class="list-group-item"><a href="#" class="text-dark fw-bold">2. Viagem espacial: Turismo além da órbita terrestre.</a></li>
                            <li class="list-group-item"><a href="#" class="text-dark fw-bold">3. Crise Hídrica: Regiões do Nordeste enfrentam seca severa.</a></li>
                            <li class="list-group-item"><a href="#" class="text-dark fw-bold">4. Lançamento Apple: Novo iPhone promete bateria para 3 dias.</a></li>
                            <li class="list-group-item"><a href="#" class="text-dark fw-bold">5. Saúde Mental: Aumento de casos de burnout em jovens.</a></li>
                        </ul>
                    </div>
                </div>

                <div class="ad-space mb-4" style="height: 300px;">
                    <p>ESPAÇO PARA ANÚNCIO (300x250/300) - Sidebar Inferior</p>
                    <p><small>(Publicidade Direta ou Outra Rede)</small></p>
                </div>

                <div class="card mb-4 p-4 shadow-sm" style="background-color: #f1f7fe;">
                    <h5 class="card-title text-dark mb-3">Receba Notícias no seu Email!</h5>
                    <p class="card-text">Assine nossa newsletter e não perca as principais manchetes do dia.</p>
                    <div class="input-group mb-3">
                        <input type="email" class="form-control" placeholder="Seu melhor e-mail" aria-label="Seu e-mail">
                        <button class="btn btn-primary" type="button">Assinar</button>
                    </div>
                    <small class="text-muted">Seu e-mail está seguro conosco. Leia nossa <a href="#" class="text-primary">Política de Privacidade</a>.</small>
                </div>

            </div>
        </div>
    </div>

    <footer class="footer">
        <div class="container text-center">
            <div class="row">
                <div class="col-md-4 mb-3">
                    <h5>Flash News</h5>
                    <p>Sua fonte confiável de notícias diárias, cobrindo os acontecimentos mais importantes do Brasil e do mundo.</p>
                </div>
                <div class="col-md-4 mb-3">
                    <h5>Navegação</h5>
                    <ul class="list-unstyled">
                        <li><a href="#" class="text-white-50">Início</a></li>
                        <li><a href="#" class="text-white-50">Política</a></li>
                        <li><a href="#" class="text-white-50">Tecnologia</a></li>
                        <li><a href="#" class="text-white-50">Esportes</a></li>
                        <li><a href="#" class="text-white-50">Contato</a></li>
                    </ul>
                </div>
                <div class="col-md-4 mb-3">
                    <h5>Informações Legais</h5>
                    <ul class="list-unstyled">
                        <li><a href="#" class="text-white-50">Política de Privacidade</a></li>
                        <li><a href="#" class="text-white-50">Termos de Uso</a></li>
                        <li><a href="#" class="text-white-50">Anuncie Conosco</a></li>
                    </ul>
                </div>
            </div>
            <hr class="border-secondary">
            <p class="mb-0">&copy; 2025 Portal Flash News. Todos os direitos reservados.</p>
            <div class="social-icons mt-3">
                <a href="#" class="text-white-50 mx-2"><i class="fab fa-facebook-f fa-lg"></i></a>
                <a href="#" class="text-white-50 mx-2"><i class="fab fa-twitter fa-lg"></i></a>
                <a href="#" class="text-white-50 mx-2"><i class="fab fa-instagram fa-lg"></i></a>
                <a href="#" class="text-white-50 mx-2"><i class="fab fa-linkedin-in fa-lg"></i></a>
            </div>
        </div>
    </footer>

    <div id="cookieConsent">
        Este site usa cookies para garantir que você obtenha a melhor experiência. Ao continuar navegando, você concorda com o uso de cookies.
        <a href="#" style="color: #007bff; text-decoration: underline; margin-left: 10px;">Saiba mais</a>
        <button id="acceptCookies">Aceitar</button>
    </div>

    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js"></script>
    <script src="https://kit.fontawesome.com/a076d05399.js" crossorigin="anonymous"></script> 
    <script>
        // Script para mostrar o banner de cookies apenas uma vez
        document.addEventListener('DOMContentLoaded', (event) => {
            if (!localStorage.getItem('cookieAccepted')) {
                document.getElementById('cookieConsent').style.display = 'block';
            }

            document.getElementById('acceptCookies').addEventListener('click', () => {
                localStorage.setItem('cookieAccepted', 'true');
                document.getElementById('cookieConsent').style.display = 'none';
            });
        });

        // Este é um placeholder para o Google AdSense. 
        // Em um site real, você colaria os códigos dos seus blocos de anúncio aqui ou usaria um plugin.
        // As tags <ins> e <script> dentro dos comentários de adsbygoogle são exemplos do que você colaria.
        // Certifique-se de substituir 'ca-pub-XXXXXXXXXXXXXX' e 'XXXXXXXXXX' pelos seus IDs reais.
    </script>
</body>
</html>
