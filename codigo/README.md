# Código do Projeto

Mantenha neste diretório todo o código fonte do projeto. 

Se necessário, descreva neste arquivo aspectos relevantes da estrutura de diretórios criada para organização do código.

----------------- agenda.html-------------------
<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8" />
  <meta http-equiv="X-UA-Compatible" content="IE=edge" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/css/bootstrap.min.css" rel="stylesheet"
    integrity="sha384-T3c6CoIi6uLrA9TneNEoa7RxnatzjcDSCmG1MXxSR1GAsXEV/Dwwykc2MPK8M2HN" crossorigin="anonymous">

  <!-- arquivos style -->
  <link rel="stylesheet" href="assets/css/styles.css">
  <link href="assets/calendar/css/style.css" rel="stylesheet">
  <link href="assets/calendar/css/darkMode.css" rel="stylesheet">

  <title>PUC Minas - Programa de Monitoria</title>
</head>
<!-- dark mode -->

<div class="toggle">
  <input id="switch" type="checkbox" name="theme">
  <label for="switch">Toggle</label>
</div>

<!-- -------- -->

<body id="body-pd">
  <div class="l-navbar" id="navbar">
    <nav class="nav">
      <div>
        <div class="nav__brand">
          <ion-icon name="menu-outline" class="nav__toggle" id="nav-toggle"></ion-icon>
          <a href="agenda.html" class="nav__logo"><img id="logo" src="assets/img/logo.png" width="15%"></a>
        </div>

        <div class="nav__list">
          <a href="painel_aluno.html" class="nav__link active">
            <ion-icon name="home-outline" class="nav__icon"></ion-icon>
            <span class="nav__name">Painel de Controle</span>
          </a>

          <a href="mensagem.html" class="nav__link">
            <ion-icon name="chatbubbles-outline" class="nav__icon"></ion-icon>
            <span class="nav__name">Mensagem</span>
          </a>

          <a href="agenda.html" class="nav__link">
            <ion-icon name="calendar-outline" class="nav__icon"></ion-icon>
            <span class="nav__name">Calendario</span>
          </a>

          <a href="https://teams.microsoft.com/dl/launcher/launcher.html?url=teams&type=meetup-join&enableMobilePage=true&suppressPrompt=true&tenantId=14cbd5a7-ec94-46ba-b314-cc0fc972a161"
            class="nav__link">
            <ion-icon name="tv" class="nav__icon"></ion-icon>
            <span class="nav__name">Teams</span>
          </a>


          <a href="ajuda.html" class="nav__link">
            <ion-icon name="help-outline" class="nav__icon"></ion-icon>
            <span class="nav__name">Ajuda</span>
          </a>

          <a href="config.html" class="nav__link">
            <ion-icon name="settings-outline" class="nav__icon"></ion-icon>
            <span class="nav__name">Configurações</span>
          </a>
        </div>
      </div>




      <div>
        <img id="foto" src="assets/img/foto.png" width="12%">
      </div>



      <a href="login.html" class="nav__link">
        <ion-icon name="log-out-outline" class="nav__icon"></ion-icon>
        <span class="nav__name">Sair</span>
      </a>
    </nav>
  </div>
  <div id="container">
    <div id="header">
      <div id="monthDisplay"></div>

      <div>
        <button id="backButton">Voltar</button>
        <button id="nextButton">Próximo</button>
      </div>

    </div>

    <div id="weekdays">
      <div>Domingo</div>
      <div>Segunda-feira</div>
      <div>Terça-feira</div>
      <div>Quarta-feira</div>
      <div>Quinta-feira</div>
      <div>Sexta-feira</div>
      <div>Sábado</div>
    </div>


    <!-- div dinamic -->
    <div id="calendar"></div>


  </div>

  <div id="newEventModal">
    <h2>Agende a mentoria:</h2>
    Nome do monitor: <input id="eventTitleInput" placeholder="Monitor" />
    Disciplina: <input id="eventDisciplinaInput" placeholder="Disciplina" />
    Tema: <input id="eventTemaInput" placeholder="Tema:" />
    Link da Reunião: <input id="eventLinkInput" placeholder="Link da Reunião" />

    <button id="saveButton"> Salvar</button>
    <button id="cancelButton">Cancelar</button>
  </div>

  <div id="deleteEventModal">
    <h2>Evento</h2>

    <div id="eventText"></div><br>


    <button id="deleteButton">Deletar</button>
    <button id="closeButton">Fechar</button>
  </div>

  <div id="modalBackDrop"></div>

  <!-- ===== IONICONS ===== -->
  <script src="https://unpkg.com/ionicons@5.1.2/dist/ionicons.js"></script>

  <!-- ===== MAIN JS ===== -->
  <script src="assets/js/main.js"></script>

  <!-- ===== BOOTSTRAP ===== -->
  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.bundle.min.js"
    integrity="sha384-C6RzsynM9kWDrMNeT87bh95OGNyZPhcTNXj1NW7RuBCsyN/o0jlpcV8Qyq46cDfL"
    crossorigin="anonymous"></script>

  <!--Calendario JS-->
  <script src="assets/calendar/scripts/darkMode.js"></script>
  <script src="assets/calendar/scripts/main.js"></script>

</body>

</html>

----------------- ajuda.html-------------------

<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.4.1/css/bootstrap.min.css">
  <script src="https://code.jquery.com/jquery-3.4.1.slim.min.js"></script>
  <script src="https://stackpath.bootstrapcdn.com/bootstrap/4.4.1/js/bootstrap.min.js"></script>
  <link rel="stylesheet" href="./style.css">
  <!-- ===== CSS ===== -->
  <link rel="stylesheet" href="assets/css/styles.css">
  <!-- ===== ICON ===== -->
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.2/css/all.min.css"
    integrity="sha512-z3gLpd7yknf1YoNbCzqRKc4qyor8gaKU1qmn+CShxbuBusANI9QpRohGBreCFkKxLhei6S9CQXFEbbKuqLg0DA=="
    crossorigin="anonymous" referrerpolicy="no-referrer" />

  <title>PUC Minas - Programa de Monitoria</title>
</head>

<body id="body-pd">
  <div class="l-navbar" id="navbar">
    <nav class="nav">
      <div>
        <div class="nav__brand">
          <ion-icon name="menu-outline" class="nav__toggle" id="nav-toggle"></ion-icon>
          <a href="ajuda.html" class="nav__logo"><img id="logo" src="assets/img/logo.png" width="15%"></a>
        </div>

        <div class="nav__list">
          <a href="painel_aluno.html" class="nav__link active">
            <ion-icon name="home-outline" class="nav__icon"></ion-icon>
            <span class="nav__name">Painel de Controle</span>
          </a>

          <a href="mensagem.html" class="nav__link">
            <ion-icon name="chatbubbles-outline" class="nav__icon"></ion-icon>
            <span class="nav__name">Mensagem</span>
          </a>

          <a href="agenda.html" class="nav__link">
            <ion-icon name="calendar-outline" class="nav__icon"></ion-icon>
            <span class="nav__name">Calendario</span>
          </a>

          <a href="https://teams.microsoft.com/dl/launcher/launcher.html?url=teams&type=meetup-join&enableMobilePage=true&suppressPrompt=true&tenantId=14cbd5a7-ec94-46ba-b314-cc0fc972a161"
            class="nav__link">
            <ion-icon name="tv" class="nav__icon"></ion-icon>
            <span class="nav__name">Teams</span>
          </a>


          <a href="ajuda.html" class="nav__link">
            <ion-icon name="help-outline" class="nav__icon"></ion-icon>
            <span class="nav__name">Ajuda</span>
          </a>

          <a href="config.html" class="nav__link">
            <ion-icon name="settings-outline" class="nav__icon"></ion-icon>
            <span class="nav__name">Configurações</span>
          </a>
        </div>
      </div>

      <div>
        <img id="foto" src="assets/img/foto.png" width="12%">
      </div>

      <a href="login.html" class="nav__link">
        <ion-icon name="log-out-outline" class="nav__icon"></ion-icon>
        <span class="nav__name">Sair</span>
      </a>
    </nav>
  </div>

  <section class="faq pt-2">
    <div class="container">
      <div class="faq-title">
        <h2>Ajuda?</h2>
        <p>Perdido, Tente aqui primeiro!</p>
      </div>

      <ul class="faq-list">
        <li data-aos="fade-up" data-aos-delay="100" class="aos-init aos-animate">
          <a data-toggle="collapse" class="collapsed" href="#faq1" aria-expanded="false">Página de Boas-vindas <i
              class="fas fa-arrow-up"></i></a>
          <div id="faq1" class="collapse" data-parent=".faq-list">
            <p>
              Bem-vindo à nossa página de ajuda! Aqui você encontrará informações e recursos para tornar sua experiência
              em nosso site mais fácil e agradável. Se tiver alguma dúvida, você veio ao lugar certo.
            </p>
          </div>
        </li>

        <li data-aos="fade-up" data-aos-delay="200" class="aos-init aos-animate">
          <a data-toggle="collapse" href="#faq2" class="collapsed">Como faço para criar uma conta em seu site?<i
              class="fas fa-arrow-up"></i></a>
          <div id="faq2" class="collapse" data-parent=".faq-list">
            <p>
              Para criar uma conta, clique no botão "Cadastre-se" na página inicial e siga as instruções. Você precisará
              fornecer seu nome, endereço de e-mail e criar uma senha.
            </p>
          </div>
        </li>

        <li data-aos="fade-up" data-aos-delay="300" class="aos-init aos-animate">
          <a data-toggle="collapse" href="#faq3" class="collapsed">Esqueci minha senha. Como posso me recuperar? <i
              class="fas fa-arrow-up"></i></a>
          <div id="faq3" class="collapse" data-parent=".faq-list">
            <p>
              Se você esqueceu sua senha, vá para a página de login e clique no link "Esqueceu sua senha?". Insira o
              endereço de e-mail associado à sua conta e siga as instruções enviadas para redefinir sua
              senha. Nao esqueca de verificar sua caixa de spam se não receber o e-mail imediatamente.
            </p>
          </div>
        </li>

        <li data-aos="fade-up" data-aos-delay="400" class="aos-init aos-animate">
          <a data-toggle="collapse" href="#faq4" class="collapsed">Como posso atualizar minhas informações de perfil? <i
              class="fas fa-arrow-up"></i></a>
          <div id="faq4" class="collapse" data-parent=".faq-list">
            <p>
              Para atualizar suas informações de perfil, faça login em sua conta e acesse a seção "Perfil",
              "Configurações". Lá, você pode editar seu nome, foto de perfil e outras informações
              pessoais. Lembre-se de salvar as alterações após fazer as edições.
            </p>
          </div>
        </li>


        <li data-aos="fade-up" data-aos-delay="500" class="aos-init aos-animate">
          <a data-toggle="collapse" href="#faq5" class="collapsed">O que devo fazer se suspeitar de atividades
            fraudulentas em minha conta? <i class="fas fa-arrow-up"></i></a>
          <div id="faq5" class="collapse" data-parent=".faq-list">
            <p>
              Se você suspeitar de atividades fraudulentas em sua conta, entre em contato conosco imediatamente. Nossa
              equipe de suporte pode ajudá-lo a garantir a segurança de sua conta, alterando sua senha, revisando suas
              atividades recentes e tomando as medidas necessárias para protegê-lo contra fraude.
            </p>
          </div>
        </li>
        
        <li data-aos="fade-up" data-aos-delay="600" class="aos-init aos-animate">
          <a data-toggle="collapse" href="#faq6" class="collapsed"> Como faço para entrar em contato com a PUC: <i class="fas fa-arrow-up"></i></a>
          <div id="faq6" class="collapse" data-parent=".faq-list">
            <p>
             Para entrar em contato com a PUC é so você clicar na imagem abaixo que você irá ser direcionado para a página de contatos da PUC.
            </p>
          </div>
        </li>
      </ul>
      <a href="https://www.pucminas.br/destaques/Paginas/funcionamento-puc-minas.aspx?fbclid=IwAR3VJpvS9OlaiIsc_Egokip8pjUnGAoqAolnYjXP_APEu9dAT8tW4ySQE-A#:~:text=Via%20email%2C%20pelo%20link%20%22Fale,%2C%20das%207h%20%C3%A0s%2017h).&text=(31)%203319%2D4525%20%2F,e%20canvas%40pucminas.br.">
      <img id="banner" src="assets/img/banner-portal-central-informacoes.jpg" class="d-block w-100"></a>
    </div>
  </section>





  <!-- ===== IONICONS ===== -->
  <script src="https://unpkg.com/ionicons@5.1.2/dist/ionicons.js"></script>

  <!-- ===== MAIN JS ===== -->
  <script src="assets/js/main.js"></script>
</body>

</html>


----------------- ATP_aluno.html-------------------
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap@4.0.0/dist/css/bootstrap.min.css"
        integrity="sha384-Gn5384xqQ1aoWXA+058RXPxPg6fy4IWvTNh0E263XmFcJlSAwiGgFAW/dAiS6JXm" crossorigin="anonymous">

    <!-- ===== CSS ===== -->
    <link rel="stylesheet" href="assets/css/styles.css">
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap@4.0.0/dist/css/bootstrap.min.css">
    <title>Conteúdos da Matéria</title>
    <script src="https://code.jquery.com/jquery-3.6.0.min.js"></script>
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@4.0.0/dist/js/bootstrap.min.js"></script>
    <style>
        .card-body iframe {
            display: block;
            margin: 0 auto;
            width: 95%;
            /* Ajuste a largura conforme necessário */
        }
    </style>

    </style>
</head>


<body id="body-pd">

    <a href="painel_aluno.html" class="btn btn-primary">Voltar</a>


    <div class="l-navbar" id="navbar">
        <nav class="nav">
            <div>
                <div class="nav__brand">
                    <ion-icon name="menu-outline" class="nav__toggle" id="nav-toggle"></ion-icon>
                    <a href="painel_aluno.html" class="nav__logo"><img id="logo" src="assets/img/logo.png"
                            width="15%"></a>
                </div>

                <div class="nav__list">
                    <a href="painel_aluno.html" class="nav__link active">
                        <ion-icon name="home-outline" class="nav__icon"></ion-icon>
                        <span class="nav__name">Painel de Controle</span>
                    </a>

                    <a href="mensagem.html" class="nav__link">
                        <ion-icon name="chatbubbles-outline" class="nav__icon"></ion-icon>
                        <span class="nav__name">Mensagem</span>
                    </a>

                    <a href="agenda.html" class="nav__link">
                        <ion-icon name="calendar-outline" class="nav__icon"></ion-icon>
                        <span class="nav__name">Calendario</span>
                    </a>

                    <a href="https://teams.microsoft.com/dl/launcher/launcher.html?url=teams&type=meetup-join&enableMobilePage=true&suppressPrompt=true&tenantId=14cbd5a7-ec94-46ba-b314-cc0fc972a161"
                        class="nav__link">
                        <ion-icon name="tv" class="nav__icon"></ion-icon>
                        <span class="nav__name">Teams</span>
                    </a>


                    <a href="ajuda.html" class="nav__link">
                        <ion-icon name="help-outline" class="nav__icon"></ion-icon>
                        <span class="nav__name">Ajuda</span>
                    </a>

                    <a href="config.html" class="nav__link">
                        <ion-icon name="settings-outline" class="nav__icon"></ion-icon>
                        <span class="nav__name">Configurações</span>
                    </a>
                </div>
            </div>


            <div>
                <img id="foto" src="assets/img/foto.png" width="12%">
            </div>

            <a href="login.html" class="nav__link">
                <ion-icon name="log-out-outline" class="nav__icon"></ion-icon>
                <span class="nav__name">Sair</span>
            </a>
        </nav>
    </div>

    <section class="container-fluid">
        <div class="titulo">
            <h1>
                <h1>Conteúdos da Matéria - ALGORITMOS E TECNICAS DE PROGRAMACAO </h1>
            </h1>
        </div>

        <!-- Conteúdo 1 -->
        <div class="card">
            <div class="card-header" id="contentHeading1">
                <h2 class="mb-0">
                    <button class="btn btn-link" type="button" data-toggle="collapse" data-target="#contentCollapse1"
                        aria-expanded="true" aria-controls="contentCollapse1">
                        Semana 1 - Condicionais "if-else" C# <ion-icon name="arrow-forward-outline"></ion-icon>
                    </button>
                </h2>
            </div>
            <div id="contentCollapse1" class="collapse" aria-labelledby="contentHeading1"
                data-parent="#contentAccordion">
                <div class="card-body">
                    <h3>O Mundo dos Condicionais "if-else" em C#: Uma Explicação Simplificada</h3>
                    <p>O condicional "if-else" é uma parte fundamental da programação em C# e em muitas outras
                        linguagens. Vamos dar uma olhada em uma explicação simplificada sobre como ele funciona.</p>
                    <h4>1. Testando Condições:</h4>
                    <p>O condicional "if-else" é como um guarda que toma decisões com base em condições. Ele começa
                        testando uma condição, que é uma expressão que pode ser verdadeira (true) ou falsa (false).</p>
                    <h4>2. O "if":</h4>
                    <p>Se a condição testada no "if" for verdadeira, um bloco de código é executado. É como tomar uma
                        ação se uma condição for atendida. Por exemplo, se você estiver chovendo, você pega um
                        guarda-chuva.</p>
                    <h4>3. O "else":</h4>
                    <p>Se a condição no "if" for falsa, você pode especificar um bloco de código para ser executado no
                        "else". Isso é como tomar uma ação alternativa se a primeira condição não for atendida. Por
                        exemplo, se você não estiver chovendo, você não pega um guarda-chuva.</p>
                    <h4>4. Tomando Decisões:</h4>
                    <p>Usando "if" e "else" em conjunto, você pode tomar decisões com base em diferentes cenários. Por
                        exemplo, se a idade de uma pessoa for maior que 18 anos, ela pode comprar bebidas alcoólicas;
                        caso contrário, não pode.</p>
                    <h4>5. "if-else if-else":</h4>
                    <p>Você também pode usar uma série de "if-else if-else" para lidar com várias condições. Isso é como
                        ter várias opções e ações baseadas em diferentes situações. Por exemplo, se estiver chovendo,
                        pegue um guarda-chuva; se estiver úmido, use óculos de sol; caso contrário, leve um casaco.</p>
                    <p>Em resumo, o condicional "if-else" em C# é uma maneira de fazer seu programa tomar decisões com
                        base em condições. Ele permite que seu código escolha entre diferentes caminhos a serem
                        seguidos, dependendo das situações. Portanto, da próxima vez que você se deparar com um
                        "if-else" em seu código, lembre-se de que ele é como um guardião que orienta seu programa a agir
                        de acordo com as condições condicionais.</p>

                    <iframe width="699" height="393" src="https://www.youtube.com/embed/Ojm98Gg1rVw"
                        title="Como a Internet chega na minha casa? - @Curso em Vídeo HTML5 e CSS3" frameborder="0"
                        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
                        allowfullscreen>
                    </iframe>
                </div>
            </div>
        </div>

        <!-- Conteudo 2 -->
        <div class="card">
            <div class="card-header" id="contentHeading2">
                <h2 class="mb-0">
                    <button class="btn btn-link" type="button" data-toggle="collapse" data-target="#contentCollapse3"
                        aria-expanded="true" aria-controls="contentCollapse3">
                        Semana 2 - "Switch-case" em C#!<ion-icon name="arrow-forward-outline"></ion-icon>
                    </button>
                </h2>
            </div>
            <div id="contentCollapse3" class="collapse" aria-labelledby="contentHeading3"
                data-parent="#contentAccordion">
                <div class="card-body">

                    <h3>Decifrando o "Switch-Case" em C#: Uma Explicação Simplificada</h3>
                    <p>O condicional "switch-case" é uma parte importante da programação em C#, que permite tomar
                        decisões com base em valores específicos. Vamos dar uma olhada em uma explicação simplificada
                        sobre como ele funciona.</p>
                    <h4>1. Avaliação de Valores:</h4>
                    <p>O "switch-case" é como um inspetor que avalia um valor específico. Ele começa observando o valor
                        de uma expressão e, em seguida, decide qual bloco de código executar com base nesse valor.</p>
                    <h4>2. O "Switch":</h4>
                    <p>O "switch" é como o inspetor de valores. Ele recebe a expressão que deseja avaliar e verificar
                        cada "caso" para ver se corresponde ao valor da expressão. É como ter várias opções disponíveis.
                    </p>
                    <h4>3. Os "Case":</h4>
                    <p>Os "case" são como etiquetas que identificam os valores específicos que o "switch" está
                        avaliando. Cada "caso" contém um valor que será comparado com a expressão. Se houver uma
                        correspondência, o bloco de código dentro desse "case" será executado.</p>
                    <h4>4. O "Default":</h4>
                    <p>Se nenhum dos "case" corresponde ao valor da expressão, você pode fornecer um "default". É como
                        uma opção de último recurso, caso nenhum dos "case" se aplique. O bloco de código dentro de
                        "default" é executado se nenhum "case" coincidir.</p>
                    <h4>5. Tomando Decisões com Valores:</h4>
                    <p>Usando "switch-case", você pode tomar decisões com base em valores específicos. Por exemplo, se a
                        expressão para o dia da semana, o "switch-case" pode determinar qual ação realizar com base no
                        dia atual.</p>
                    <p>
                        Em resumo, o condicional "switch-case" em C# é uma maneira de direcionar seu programa para
                        diferentes blocos de código com base em valores específicos. É como ter várias opções
                        disponíveis e escolher a ação com base no valor da expressão. Portanto, da próxima vez que você
                        encontrar um "switch-case" em seu código, lembre-se de que ele é como um inspetor que orienta
                        seu programa com base nos valores fornecidos.</p>


                    <iframe width="699" height="393" src="https://www.youtube.com/embed/v2H1MNSkE_s"
                        title="A diferença entre HTML, CSS e JavaScript - @Curso em Vídeo HTML5 e CSS3" frameborder="0"
                        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
                        allowfullscreen>
                    </iframe>
                </div>
            </div>
        </div>

        <!-- Conteúdo 3 -->
        <div class="card">
            <div class="card-header" id="contentHeading3">
                <h2 class="mb-0">
                    <button class="btn btn-link" type="button" data-toggle="collapse" data-target="#contentCollapse4"
                        aria-expanded="true" aria-controls="contentCollapse4">
                        Semana 3 - Estruturas de Repetição (for) c# <ion-icon name="arrow-forward-outline"></ion-icon>
                    </button>
                </h2>
            </div>
            <div id="contentCollapse4" class="collapse" aria-labelledby="contentHeading4"
                data-parent="#contentAccordion">
                <div class="card-body">


                    <h3>Explorando a Estrutura de Repetição "for" em C#: Uma Explicação Simplificada</h3>
                    <p>A estrutura de repetição "for" é uma parte importante da programação em C#, que permite executar
                        um bloco de código várias vezes. Vamos dar uma olhada em uma explicação simplificada sobre como
                        ela funciona.</p>

                    <h4>1. Contagem e Controle:</h4>
                    <p>O "for" é como um contador e controlador de repetições. Ele começa especificando uma variável de
                        controle, uma condição de continuação e um incremento (ou decremento). A variável de controle é
                        como o contador.</p>

                    <h4>2. Inicialização da Variável de Controle:</h4>
                    <p>O "for" inicia a variável de controle com um valor inicial. Isso é como definir o ponto de
                        partida do contador. Por exemplo, começando com 1.</p>

                    <h4>3. Condição de Continuação:</h4>
                    <p>O "for" estabelece uma condição que determina quando a repetição deve parar. Enquanto a condição
                        for verdadeira, o bloco de código é executado repetidamente. É como dizer até onde o contador
                        deve ir. Por exemplo, continue até que o contador seja menor ou igual a 10.</p>

                    <h4>4. Incremento/Decremento da Variável de Controle:</h4>
                    <p>O "for" especifica como a variável de controle deve ser alterada a cada repetição. Isso é como
                        dizer como o contador deve ser atualizado após cada execução do bloco de código. Por exemplo,
                        aumentar o contador em 1 a cada repetição.</p>

                    <h4>5. Realizando Tarefas Repetitivas:</h4>
                    <p>Usando "for", você pode realizar tarefas repetitivas, como percorrer uma lista de itens, imprimir
                        valores sequenciais ou realizar cálculos repetidos.</p>

                    <h4>6. Parando a Repetição:</h4>
                    <p>Quando a condição de continuação não for mais atendida, a repetição para. É como dizer ao
                        contador para parar quando atingir um determinado limite.</p>

                    <p>Em resumo, a estrutura de repetição "for" em C# é uma maneira de executar um bloco de código
                        várias vezes, controlando o processo por meio de uma variável de controle, uma condição de
                        continuação e um incremento. É como automatizar tarefas repetitivas de maneira eficiente.
                        Portanto, da próxima vez que você usar um "for" em seu código, lembre-se de que ele é como um
                        contador que realiza uma ação específica um número determinado de vezes.</p>



                    <iframe width="699" height="393" src="https://www.youtube.com/embed/GoQLs_sJLXs"
                        title="Front-end, Back-end e Full stack - @Curso em Vídeo HTML5 e CSS3" frameborder="0"
                        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
                        allowfullscreen></iframe>
                </div>
            </div>
        </div>


        <!-- Conteúdo 4 -->
        <div class="card">
            <div class="card-header" id="contentHeading4">
                <h2 class="mb-0">
                    <button class="btn btn-link" type="button" data-toggle="collapse" data-target="#contentCollapse5"
                        aria-expanded="true" aria-controls="contentCollapse5">
                        Semana 4 - Estruturas de Repetição (while) c# <ion-icon name="arrow-forward-outline"></ion-icon>
                    </button>
                </h2>
            </div>
            <div id="contentCollapse5" class="collapse" aria-labelledby="contentHeading5"
                data-parent="#contentAccordion">
                <div class="card-body">

                    <h3>Explorando a Estrutura de Repetição "while" em C#:</h3>
                    <p>A estrutura de repetição "while" é uma parte importante da programação em C#, que permite
                        executar um bloco de código repetidamente enquanto uma condição específica for verdadeira. Vamos
                        dar uma olhada em uma explicação simplificada, com base no material da Profa. Soraia, sobre como
                        ela funciona.</p>

                    <h4>1. Requisitos e Continuidade:</h4>
                    <p>O "while" é como um segurança que fica de olho em uma condição. Ele começa especificando uma
                        condição que deve ser verdadeira para continuar a execução do bloco de código. A repetição
                        acontece enquanto a condição for verdadeira.</p>

                    <h4>2. Avaliação Inicial:</h4>
                    <p>O "while" avalia a condição antes de executar o bloco de código. Se a condição for verdadeira
                        desde o início, o bloco é executado. Se a condição for falsa desde o início, o bloco pode nunca
                        ser executado.</p>

                    <h4>3. Atualização da Condição:</h4>
                    <p>O "while" não atualiza automaticamente a condição. Você precisa garantir que dentro do bloco de
                        código exista alguma lógica que possa, eventualmente, tornar a condição falsa. Caso contrário, a
                        repetição pode se tornar infinita.</p>

                    <h4>4. Realizando Tarefas Repetitivas:</h4>
                    <p>Usando "while", você pode realizar tarefas repetitivas, como processar dados em uma lista,
                        interagir com o usuário até que ele forneça uma resposta válida ou executar uma ação até que uma
                        determinada condição seja atendida.</p>

                    <h4>5. Controle Fino:</h4>
                    <p>O "while" oferece um controle fino sobre quando a repetição começa e para. Você pode personalizar
                        a condição e o momento em que a repetição ocorre, tornando-o adequado para situações em que a
                        lógica de repetição é complexa.</p>

                    <p>Em resumo, a estrutura de repetição "while" em C#, com base no material da Profa. Soraia, é uma
                        maneira de executar um bloco de código repetidamente, contanto que uma condição específica seja
                        atendida. Ela permite uma abordagem flexível para realizar tarefas repetitivas e exige que você
                        controle explicitamente a condição de parada. Portanto, da próxima vez que você usar um "while"
                        em seu código, lembre-se de que ele é como um segurança que mantém um olhar atento sobre uma
                        condição antes de permitir a execução do bloco.</p>


                    <iframe width="699" height="393" src="https://www.youtube.com/embed/P5OiZFmG8bc"
                        title="Título do Vídeo 5" frameborder="0"
                        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
                        allowfullscreen>
                    </iframe>
                </div>
            </div>
        </div>

        <!-- Conteúdo 5 -->
        <div class="card">
            <div class="card-header" id="contentHeading5">
                <h2 class="mb-0">
                    <button class="btn btn-link" type="button" data-toggle="collapse" data-target="#contentCollapse6"
                        aria-expanded="true" aria-controls="contentCollapse6">
                        Semana 5 - Estruturas de Repetição (do-while) <ion-icon name="arrow-forward-outline"></ion-icon>
                    </button>
                </h2>
            </div>
            <div id="contentCollapse5" class="collapse" aria-labelledby="contentHeading5"
                data-parent="#contentAccordion">
                <div class="card-body">


                    <h3>Desvendando a Estrutura de Repetição "do-while" em C#: Uma Explicação Simplificada</h3>
                    <p>A estrutura de repetição "do-while" é uma parte essencial da programação em C#, permitindo que
                        você execute um bloco de código repetidamente com base em uma condição específica. Vamos
                        explorar uma explicação simplificada sobre como ela funciona.</p>

                    <h4>1. Execução Garantida:</h4>
                    <p>O "do-while" é como um anfitrião que convida você para a festa antes mesmo de verificar quem está
                        presente. Ele começa executando o bloco de código pelo menos uma vez, independentemente da
                        condição.</p>

                    <h4>2. Avaliação da Condição:</h4>
                    <p>Após a primeira execução do bloco de código, o "do-while" avalia a condição. Se a condição for
                        verdadeira, o bloco de código é executado novamente. Caso contrário, a repetição para.</p>

                    <h4>3. Controle Fino e Atualização:</h4>
                    <p>O "do-while" oferece controle refinado, permitindo que você personalize a condição e o momento em
                        que a repetição ocorre. Você deve garantir que dentro do bloco de código exista lógica que
                        possa, eventualmente, tornar a condição falsa, para evitar repetições infinitas.</p>

                    <h4>4. Realizando Tarefas Repetitivas:</h4>
                    <p>Usando "do-while", você pode realizar tarefas repetitivas, como interagir com o usuário até que
                        ele forneça uma resposta válida ou processar dados em uma lista até que uma determinada condição
                        seja atendida.</p>

                    <h4>5. Útil para Validações:</h4>
                    <p>O "do-while" é especialmente útil para situações em que você deseja garantir que um bloco de
                        código seja executado pelo menos uma vez antes de verificar uma condição, o que é comum em
                        validações de entrada de dados.</p>

                    <p>Em resumo, a estrutura de repetição "do-while" em C# é uma maneira de executar um bloco de código
                        repetidamente, garantindo que ele seja executado pelo menos uma vez. Ela permite um controle
                        preciso sobre a condição de parada e é útil em cenários em que você precisa validar dados ou
                        realizar ações repetidas. Portanto, da próxima vez que você usar um "do-while" em seu código,
                        lembre-se de que ele é como um anfitrião que convida você para a festa antes mesmo de saber quem
                        está presente, mas garante que todos tenham a chance de participar.</p>



                    <iframe width="699" height="393" src="https://www.youtube.com/embed/mb-r3-A6yYo"
                        title="Título do Vídeo 5" frameborder="0"
                        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
                        allowfullscreen>
                    </iframe>
                </div>
            </div>
        </div>


        <!-- Conteúdo 6 -->
        <div class="card">
            <div class="card-header" id="contentHeading6">
                <h2 class="mb-0">
                    <button class="btn btn-link" type="button" data-toggle="collapse" data-target="#contentCollapse6"
                        aria-expanded="true" aria-controls="contentCollapse6">
                        Semana 6 - Vetores (arrays) em c# <ion-icon name="arrow-forward-outline"></ion-icon>
                    </button>
                </h2>
            </div>
            <div id="contentCollapse6" class="collapse" aria-labelledby="contentHeading6"
                data-parent="#contentAccordion">
                <div class="card-body">

                    <h3>Explorando Vetores em C#: Uma Explicação Simplificada</h3>
                    <p>Vetores são uma estrutura de dados essencial em C# que permite armazenar uma coleção de elementos
                        do mesmo tipo. Vamos dar uma olhada em uma explicação simplificada sobre como eles funcionam.
                    </p>

                    <h4>1. Coleção de Elementos:</h4>
                    <p>Um vetor é como uma coleção de elementos semelhantes organizados em sequência. Esses elementos
                        podem ser números, textos, objetos ou qualquer outro tipo de dado suportado pela linguagem.</p>

                    <h4>2. Índices Numéricos:</h4>
                    <p>Cada elemento em um vetor é identificado por um índice numérico. Os índices começam em 0 para o
                        primeiro elemento, 1 para o segundo elemento e assim por diante. O índice ajuda a acessar e
                        manipular elementos específicos no vetor.</p>

                    <h4>3. Tamanho Fixo:</h4>
                    <p>Os vetores em C# têm um tamanho fixo, o que significa que você precisa especificar o número de
                        elementos que o vetor conterá quando o criar. Após a criação, o tamanho não pode ser alterado.
                    </p>

                    <h4>4. Declaração e Inicialização:</h4>
                    <p>Para criar um vetor, você deve declará-lo e inicializá-lo. A declaração informa ao compilador o
                        tipo de dado que o vetor conterá, enquanto a inicialização define o tamanho e, opcionalmente,
                        atribui valores iniciais aos elementos.</p>

                    <h4>5. Acesso aos Elementos:</h4>
                    <p>Você pode acessar elementos individuais em um vetor usando seus índices. Por exemplo, se você
                        tiver um vetor de inteiros, pode acessar o terceiro elemento usando o índice 2: `vetor[2]`.</p>

                    <h4>6. Manipulação de Dados:</h4>
                    <p>Vetores permitem que você armazene, modifique e recupere dados de forma eficiente. Isso é útil
                        para lidar com coleções de dados, como listas de compras, notas de alunos ou informações de
                        contato.</p>

                    <h4>7. Laços de Repetição:</h4>
                    <p>Os vetores são frequentemente combinados com estruturas de repetição, como "for" ou "foreach",
                        para processar todos os elementos de um vetor de maneira iterativa.</p>

                    <p>Em resumo, vetores em C# são uma maneira de armazenar e manipular coleções de elementos do mesmo
                        tipo. Eles são especialmente úteis quando você precisa lidar com um grupo de dados relacionados
                        e deseja acessar ou modificar esses dados de forma eficiente. Portanto, da próxima vez que você
                        trabalhar com vetores em seu código, lembre-se de que eles são como um conjunto ordenado de
                        elementos, cada um acessado por um índice numérico.</p>


                    <iframe width="699" height="393" src="https://www.youtube.com/embed/utkQHvmmJ38"
                        title="Título do Vídeo 6" frameborder="0"
                        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
                        allowfullscreen>
                    </iframe>
                </div>
            </div>
        </div>


    </section>

    <script src="https://unpkg.com/ionicons@5.1.2/dist/ionicons.js"></script>
    <script src="assets/js/main.js"></script>
    <script src="assets/js/materias.js"></script>


    <!-- ===== IONICONS ===== -->
    <script src="https://unpkg.com/ionicons@5.1.2/dist/ionicons.js"></script>

    <!-- ===== MAIN JS ===== -->
    <script src="assets/js/main.js"></script>

    <!-- ===== BOOTSTRAP ===== -->
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@4.0.0/dist/js/bootstrap.min.js"
        integrity="sha384-JZR6Spejh4U02d8jOt6vLEHfe/JQGiRRSQQxSfFWpi1MquVdAyjUar5+76PVCmYl" crossorigin="anonymous">
        </script>

</body>

</html>

------------------ ATP_Monitor.html-------------------
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap@4.0.0/dist/css/bootstrap.min.css"
        integrity="sha384-Gn5384xqQ1aoWXA+058RXPxPg6fy4IWvTNh0E263XmFcJlSAwiGgFAW/dAiS6JXm" crossorigin="anonymous">

    <!-- ===== CSS ===== -->
    <link rel="stylesheet" href="assets/css/styles.css">
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap@4.0.0/dist/css/bootstrap.min.css">
    <title>Conteúdos da Matéria</title>
    <script src="https://code.jquery.com/jquery-3.6.0.min.js"></script>
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@4.0.0/dist/js/bootstrap.min.js"></script>

<style>
    .card-body iframe {
            display: block;
            margin: 0 auto;
            width: 95%;
            /* Ajuste a largura conforme necessário */
        }

    .edit-btn,
   .delete-btn {
       position: absolute;
       top: 5px;
       z-index: 999;
       padding: 0.2rem 0.4rem;
       font-size: 0.75rem;
   }

   .edit-btn ion-icon,
   .delete-btn ion-icon {
       font-size: 1rem;
   }

   .edit-btn {
       right: 40px; /* Distância da borda direita para o botão de edição */
   }

   .delete-btn {
       right: 5px; /* Distância da borda direita para o botão de exclusão */
   }

   .card-header {
       position: relative;
   }
</style>

</head>


<body id="body-pd">

    <a href="painel_monitor.html" class="btn btn-primary">Voltar</a>
    

    <div class="l-navbar" id="navbar">
        <nav class="nav">
            <div>
                <div class="nav__brand">
                    <ion-icon name="menu-outline" class="nav__toggle" id="nav-toggle"></ion-icon>
                    <a href="painel_aluno.html" class="nav__logo"><img id="logo" src="assets/img/logo.png"
                            width="15%"></a>
                </div>

                <div class="nav__list">
                    <a href="painel_monitor.html" class="nav__link active">
                        <ion-icon name="home-outline" class="nav__icon"></ion-icon>
                        <span class="nav__name">Painel de Controle</span>
                    </a>

                    <a href="mensagem.html" class="nav__link">
                        <ion-icon name="chatbubbles-outline" class="nav__icon"></ion-icon>
                        <span class="nav__name">Mensagem</span>
                    </a>

                    <a href="agenda.html" class="nav__link">
                        <ion-icon name="calendar-outline" class="nav__icon"></ion-icon>
                        <span class="nav__name">Calendario</span>
                    </a>

                    <a href="https://teams.microsoft.com/dl/launcher/launcher.html?url=teams&type=meetup-join&enableMobilePage=true&suppressPrompt=true&tenantId=14cbd5a7-ec94-46ba-b314-cc0fc972a161"
                        class="nav__link">
                        <ion-icon name="tv" class="nav__icon"></ion-icon>
                        <span class="nav__name">Teams</span>
                    </a>


                    <a href="ajuda.html" class="nav__link">
                        <ion-icon name="help-outline" class="nav__icon"></ion-icon>
                        <span class="nav__name">Ajuda</span>
                    </a>

                    <a href="config.html" class="nav__link">
                        <ion-icon name="settings-outline" class="nav__icon"></ion-icon>
                        <span class="nav__name">Configurações</span>
                    </a>
                </div>
            </div>


            <div>
                <img id="foto" src="assets/img/foto.png" width="15%">
            </div>

            <a href="login.html" class="nav__link">
                <ion-icon name="log-out-outline" class="nav__icon"></ion-icon>
                <span class="nav__name">Sair</span>
            </a>
        </nav>
    </div>

    <section class="container-fluid">
        <div class="titulo">
            <h1>
                <h1>Conteúdos da Matéria - ALGORITMOS E TECNICAS DE PROGRAMACAO </h1>
            </h1>
        </div>

        <!-- Conteúdo 1 -->
        <div class="card">
            <div class="card-header position-relative" id="contentHeading1">
                <button class="btn btn-primary edit-btn"><ion-icon name="create-outline"></ion-icon></button>
                <button class="btn btn-danger delete-btn"><ion-icon name="trash-outline"></ion-icon></button>
                <h2 class="mb-0">
                    <button class="btn btn-link" type="button" data-toggle="collapse" data-target="#contentCollapse1"
                        aria-expanded="true" aria-controls="contentCollapse1">
                        Semana 1 - Condicionais "if-else" C# <ion-icon name="arrow-forward-outline"></ion-icon>
                    </button>
                </h2>
            </div>
            <div id="contentCollapse1" class="collapse" aria-labelledby="contentHeading1"
                data-parent="#contentAccordion">
                <div class="card-body">
                    <h3>O Mundo dos Condicionais "if-else" em C#: Uma Explicação Simplificada</h3>
                    <p>O condicional "if-else" é uma parte fundamental da programação em C# e em muitas outras
                        linguagens. Vamos dar uma olhada em uma explicação simplificada sobre como ele funciona.</p>
                    <h4>1. Testando Condições:</h4>
                    <p>O condicional "if-else" é como um guarda que toma decisões com base em condições. Ele começa
                        testando uma condição, que é uma expressão que pode ser verdadeira (true) ou falsa (false).</p>
                    <h4>2. O "if":</h4>
                    <p>Se a condição testada no "if" for verdadeira, um bloco de código é executado. É como tomar uma
                        ação se uma condição for atendida. Por exemplo, se você estiver chovendo, você pega um
                        guarda-chuva.</p>
                    <h4>3. O "else":</h4>
                    <p>Se a condição no "if" for falsa, você pode especificar um bloco de código para ser executado no
                        "else". Isso é como tomar uma ação alternativa se a primeira condição não for atendida. Por
                        exemplo, se você não estiver chovendo, você não pega um guarda-chuva.</p>
                    <h4>4. Tomando Decisões:</h4>
                    <p>Usando "if" e "else" em conjunto, você pode tomar decisões com base em diferentes cenários. Por
                        exemplo, se a idade de uma pessoa for maior que 18 anos, ela pode comprar bebidas alcoólicas;
                        caso contrário, não pode.</p>
                    <h4>5. "if-else if-else":</h4>
                    <p>Você também pode usar uma série de "if-else if-else" para lidar com várias condições. Isso é como
                        ter várias opções e ações baseadas em diferentes situações. Por exemplo, se estiver chovendo,
                        pegue um guarda-chuva; se estiver úmido, use óculos de sol; caso contrário, leve um casaco.</p>
                    <p>Em resumo, o condicional "if-else" em C# é uma maneira de fazer seu programa tomar decisões com
                        base em condições. Ele permite que seu código escolha entre diferentes caminhos a serem
                        seguidos, dependendo das situações. Portanto, da próxima vez que você se deparar com um
                        "if-else" em seu código, lembre-se de que ele é como um guardião que orienta seu programa a agir
                        de acordo com as condições condicionais.</p>

                    <iframe width="699" height="393" src="https://www.youtube.com/embed/Ojm98Gg1rVw"
                        title="Como a Internet chega na minha casa? - @Curso em Vídeo HTML5 e CSS3" frameborder="0"
                        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
                        allowfullscreen>
                    </iframe>
                </div>
            </div>
        </div>

        <!-- Conteudo 2 -->
        <div class="card">
            <div class="card-header position-relative" id="contentHeading1">
                <button class="btn btn-primary edit-btn"><ion-icon name="create-outline"></ion-icon></button>
                <button class="btn btn-danger delete-btn"><ion-icon name="trash-outline"></ion-icon></button>
                <h2 class="mb-0">
                    <button class="btn btn-link" type="button" data-toggle="collapse" data-target="#contentCollapse3"
                        aria-expanded="true" aria-controls="contentCollapse3">
                        Semana 2 - "Switch-case" em C#!<ion-icon name="arrow-forward-outline"></ion-icon>
                    </button>
                </h2>
            </div>
            <div id="contentCollapse3" class="collapse" aria-labelledby="contentHeading3"
                data-parent="#contentAccordion">
                <div class="card-body">

                    <h3>Decifrando o "Switch-Case" em C#: Uma Explicação Simplificada</h3>
                    <p>O condicional "switch-case" é uma parte importante da programação em C#, que permite tomar
                        decisões com base em valores específicos. Vamos dar uma olhada em uma explicação simplificada
                        sobre como ele funciona.</p>
                    <h4>1. Avaliação de Valores:</h4>
                    <p>O "switch-case" é como um inspetor que avalia um valor específico. Ele começa observando o valor
                        de uma expressão e, em seguida, decide qual bloco de código executar com base nesse valor.</p>
                    <h4>2. O "Switch":</h4>
                    <p>O "switch" é como o inspetor de valores. Ele recebe a expressão que deseja avaliar e verificar
                        cada "caso" para ver se corresponde ao valor da expressão. É como ter várias opções disponíveis.
                    </p>
                    <h4>3. Os "Case":</h4>
                    <p>Os "case" são como etiquetas que identificam os valores específicos que o "switch" está
                        avaliando. Cada "caso" contém um valor que será comparado com a expressão. Se houver uma
                        correspondência, o bloco de código dentro desse "case" será executado.</p>
                    <h4>4. O "Default":</h4>
                    <p>Se nenhum dos "case" corresponde ao valor da expressão, você pode fornecer um "default". É como
                        uma opção de último recurso, caso nenhum dos "case" se aplique. O bloco de código dentro de
                        "default" é executado se nenhum "case" coincidir.</p>
                    <h4>5. Tomando Decisões com Valores:</h4>
                    <p>Usando "switch-case", você pode tomar decisões com base em valores específicos. Por exemplo, se a
                        expressão para o dia da semana, o "switch-case" pode determinar qual ação realizar com base no
                        dia atual.</p>
                    <p>
                        Em resumo, o condicional "switch-case" em C# é uma maneira de direcionar seu programa para
                        diferentes blocos de código com base em valores específicos. É como ter várias opções
                        disponíveis e escolher a ação com base no valor da expressão. Portanto, da próxima vez que você
                        encontrar um "switch-case" em seu código, lembre-se de que ele é como um inspetor que orienta
                        seu programa com base nos valores fornecidos.</p>


                    <iframe width="699" height="393" src="https://www.youtube.com/embed/v2H1MNSkE_s"
                        title="A diferença entre HTML, CSS e JavaScript - @Curso em Vídeo HTML5 e CSS3" frameborder="0"
                        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
                        allowfullscreen>
                    </iframe>
                </div>
            </div>
        </div>

        <!-- Conteúdo 3 -->
        <div class="card">
            <div class="card-header position-relative" id="contentHeading1">
                <button class="btn btn-primary edit-btn"><ion-icon name="create-outline"></ion-icon></button>
                <button class="btn btn-danger delete-btn"><ion-icon name="trash-outline"></ion-icon></button>
                <h2 class="mb-0">
                    <button class="btn btn-link" type="button" data-toggle="collapse" data-target="#contentCollapse4"
                        aria-expanded="true" aria-controls="contentCollapse4">
                        Semana 3 - Estruturas de Repetição (for) c# <ion-icon name="arrow-forward-outline"></ion-icon>
                    </button>
                </h2>
            </div>
            <div id="contentCollapse4" class="collapse" aria-labelledby="contentHeading4"
                data-parent="#contentAccordion">
                <div class="card-body">


                    <h3>Explorando a Estrutura de Repetição "for" em C#: Uma Explicação Simplificada</h3>
                    <p>A estrutura de repetição "for" é uma parte importante da programação em C#, que permite executar
                        um bloco de código várias vezes. Vamos dar uma olhada em uma explicação simplificada sobre como
                        ela funciona.</p>

                    <h4>1. Contagem e Controle:</h4>
                    <p>O "for" é como um contador e controlador de repetições. Ele começa especificando uma variável de
                        controle, uma condição de continuação e um incremento (ou decremento). A variável de controle é
                        como o contador.</p>

                    <h4>2. Inicialização da Variável de Controle:</h4>
                    <p>O "for" inicia a variável de controle com um valor inicial. Isso é como definir o ponto de
                        partida do contador. Por exemplo, começando com 1.</p>

                    <h4>3. Condição de Continuação:</h4>
                    <p>O "for" estabelece uma condição que determina quando a repetição deve parar. Enquanto a condição
                        for verdadeira, o bloco de código é executado repetidamente. É como dizer até onde o contador
                        deve ir. Por exemplo, continue até que o contador seja menor ou igual a 10.</p>

                    <h4>4. Incremento/Decremento da Variável de Controle:</h4>
                    <p>O "for" especifica como a variável de controle deve ser alterada a cada repetição. Isso é como
                        dizer como o contador deve ser atualizado após cada execução do bloco de código. Por exemplo,
                        aumentar o contador em 1 a cada repetição.</p>

                    <h4>5. Realizando Tarefas Repetitivas:</h4>
                    <p>Usando "for", você pode realizar tarefas repetitivas, como percorrer uma lista de itens, imprimir
                        valores sequenciais ou realizar cálculos repetidos.</p>

                    <h4>6. Parando a Repetição:</h4>
                    <p>Quando a condição de continuação não for mais atendida, a repetição para. É como dizer ao
                        contador para parar quando atingir um determinado limite.</p>

                    <p>Em resumo, a estrutura de repetição "for" em C# é uma maneira de executar um bloco de código
                        várias vezes, controlando o processo por meio de uma variável de controle, uma condição de
                        continuação e um incremento. É como automatizar tarefas repetitivas de maneira eficiente.
                        Portanto, da próxima vez que você usar um "for" em seu código, lembre-se de que ele é como um
                        contador que realiza uma ação específica um número determinado de vezes.</p>



                    <iframe width="699" height="393" src="https://www.youtube.com/embed/GoQLs_sJLXs"
                        title="Front-end, Back-end e Full stack - @Curso em Vídeo HTML5 e CSS3" frameborder="0"
                        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
                        allowfullscreen></iframe>
                </div>
            </div>
        </div>


        <!-- Conteúdo 4 -->
        <div class="card">
            <div class="card-header position-relative" id="contentHeading1">
                <button class="btn btn-primary edit-btn"><ion-icon name="create-outline"></ion-icon></button>
                <button class="btn btn-danger delete-btn"><ion-icon name="trash-outline"></ion-icon></button>
                <h2 class="mb-0">
                    <button class="btn btn-link" type="button" data-toggle="collapse" data-target="#contentCollapse5"
                        aria-expanded="true" aria-controls="contentCollapse5">
                        Semana 4 - Estruturas de Repetição (while) c# <ion-icon name="arrow-forward-outline"></ion-icon>
                    </button>
                </h2>
            </div>
            <div id="contentCollapse5" class="collapse" aria-labelledby="contentHeading5"
                data-parent="#contentAccordion">
                <div class="card-body">

                    <h3>Explorando a Estrutura de Repetição "while" em C#:</h3>
                    <p>A estrutura de repetição "while" é uma parte importante da programação em C#, que permite
                        executar um bloco de código repetidamente enquanto uma condição específica for verdadeira. Vamos
                        dar uma olhada em uma explicação simplificada, com base no material da Profa. Soraia, sobre como
                        ela funciona.</p>

                    <h4>1. Requisitos e Continuidade:</h4>
                    <p>O "while" é como um segurança que fica de olho em uma condição. Ele começa especificando uma
                        condição que deve ser verdadeira para continuar a execução do bloco de código. A repetição
                        acontece enquanto a condição for verdadeira.</p>

                    <h4>2. Avaliação Inicial:</h4>
                    <p>O "while" avalia a condição antes de executar o bloco de código. Se a condição for verdadeira
                        desde o início, o bloco é executado. Se a condição for falsa desde o início, o bloco pode nunca
                        ser executado.</p>

                    <h4>3. Atualização da Condição:</h4>
                    <p>O "while" não atualiza automaticamente a condição. Você precisa garantir que dentro do bloco de
                        código exista alguma lógica que possa, eventualmente, tornar a condição falsa. Caso contrário, a
                        repetição pode se tornar infinita.</p>

                    <h4>4. Realizando Tarefas Repetitivas:</h4>
                    <p>Usando "while", você pode realizar tarefas repetitivas, como processar dados em uma lista,
                        interagir com o usuário até que ele forneça uma resposta válida ou executar uma ação até que uma
                        determinada condição seja atendida.</p>

                    <h4>5. Controle Fino:</h4>
                    <p>O "while" oferece um controle fino sobre quando a repetição começa e para. Você pode personalizar
                        a condição e o momento em que a repetição ocorre, tornando-o adequado para situações em que a
                        lógica de repetição é complexa.</p>

                    <p>Em resumo, a estrutura de repetição "while" em C#, com base no material da Profa. Soraia, é uma
                        maneira de executar um bloco de código repetidamente, contanto que uma condição específica seja
                        atendida. Ela permite uma abordagem flexível para realizar tarefas repetitivas e exige que você
                        controle explicitamente a condição de parada. Portanto, da próxima vez que você usar um "while"
                        em seu código, lembre-se de que ele é como um segurança que mantém um olhar atento sobre uma
                        condição antes de permitir a execução do bloco.</p>


                    <iframe width="699" height="393" src="https://www.youtube.com/embed/P5OiZFmG8bc"
                        title="Título do Vídeo 5" frameborder="0"
                        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
                        allowfullscreen>
                    </iframe>
                </div>
            </div>
        </div>

        <!-- Conteúdo 5 -->
        <div class="card">
            <div class="card-header position-relative" id="contentHeading1">
                <button class="btn btn-primary edit-btn"><ion-icon name="create-outline"></ion-icon></button>
                <button class="btn btn-danger delete-btn"><ion-icon name="trash-outline"></ion-icon></button>
                <h2 class="mb-0">
                    <button class="btn btn-link" type="button" data-toggle="collapse" data-target="#contentCollapse6"
                        aria-expanded="true" aria-controls="contentCollapse6">
                        Semana 5 - Estruturas de Repetição (do-while) <ion-icon name="arrow-forward-outline"></ion-icon>
                    </button>
                </h2>
            </div>
            <div id="contentCollapse5" class="collapse" aria-labelledby="contentHeading5"
                data-parent="#contentAccordion">
                <div class="card-body">


                    <h3>Desvendando a Estrutura de Repetição "do-while" em C#: Uma Explicação Simplificada</h3>
                    <p>A estrutura de repetição "do-while" é uma parte essencial da programação em C#, permitindo que
                        você execute um bloco de código repetidamente com base em uma condição específica. Vamos
                        explorar uma explicação simplificada sobre como ela funciona.</p>

                    <h4>1. Execução Garantida:</h4>
                    <p>O "do-while" é como um anfitrião que convida você para a festa antes mesmo de verificar quem está
                        presente. Ele começa executando o bloco de código pelo menos uma vez, independentemente da
                        condição.</p>

                    <h4>2. Avaliação da Condição:</h4>
                    <p>Após a primeira execução do bloco de código, o "do-while" avalia a condição. Se a condição for
                        verdadeira, o bloco de código é executado novamente. Caso contrário, a repetição para.</p>

                    <h4>3. Controle Fino e Atualização:</h4>
                    <p>O "do-while" oferece controle refinado, permitindo que você personalize a condição e o momento em
                        que a repetição ocorre. Você deve garantir que dentro do bloco de código exista lógica que
                        possa, eventualmente, tornar a condição falsa, para evitar repetições infinitas.</p>

                    <h4>4. Realizando Tarefas Repetitivas:</h4>
                    <p>Usando "do-while", você pode realizar tarefas repetitivas, como interagir com o usuário até que
                        ele forneça uma resposta válida ou processar dados em uma lista até que uma determinada condição
                        seja atendida.</p>

                    <h4>5. Útil para Validações:</h4>
                    <p>O "do-while" é especialmente útil para situações em que você deseja garantir que um bloco de
                        código seja executado pelo menos uma vez antes de verificar uma condição, o que é comum em
                        validações de entrada de dados.</p>

                    <p>Em resumo, a estrutura de repetição "do-while" em C# é uma maneira de executar um bloco de código
                        repetidamente, garantindo que ele seja executado pelo menos uma vez. Ela permite um controle
                        preciso sobre a condição de parada e é útil em cenários em que você precisa validar dados ou
                        realizar ações repetidas. Portanto, da próxima vez que você usar um "do-while" em seu código,
                        lembre-se de que ele é como um anfitrião que convida você para a festa antes mesmo de saber quem
                        está presente, mas garante que todos tenham a chance de participar.</p>



                    <iframe width="699" height="393" src="https://www.youtube.com/embed/mb-r3-A6yYo"
                        title="Título do Vídeo 5" frameborder="0"
                        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
                        allowfullscreen>
                    </iframe>
                </div>
            </div>
        </div>


              <!-- Conteúdo 6 -->
              <div class="card-header position-relative" id="contentHeading1">
                <button class="btn btn-primary edit-btn"><ion-icon name="create-outline"></ion-icon></button>
                <button class="btn btn-danger delete-btn"><ion-icon name="trash-outline"></ion-icon></button>
                <h2 class="mb-0">
                        <button class="btn btn-link" type="button" data-toggle="collapse" data-target="#contentCollapse6"
                            aria-expanded="true" aria-controls="contentCollapse6">
                            Semana 6 - Vetores (arrays) em c# <ion-icon name="arrow-forward-outline"></ion-icon>
                        </button>
                    </h2>
                </div>
                <div id="contentCollapse6" class="collapse" aria-labelledby="contentHeading6"
                    data-parent="#contentAccordion">
                    <div class="card-body">
    
                        <h3>Explorando Vetores em C#: Uma Explicação Simplificada</h3>
                        <p>Vetores são uma estrutura de dados essencial em C# que permite armazenar uma coleção de elementos
                            do mesmo tipo. Vamos dar uma olhada em uma explicação simplificada sobre como eles funcionam.
                        </p>
    
                        <h4>1. Coleção de Elementos:</h4>
                        <p>Um vetor é como uma coleção de elementos semelhantes organizados em sequência. Esses elementos
                            podem ser números, textos, objetos ou qualquer outro tipo de dado suportado pela linguagem.</p>
    
                        <h4>2. Índices Numéricos:</h4>
                        <p>Cada elemento em um vetor é identificado por um índice numérico. Os índices começam em 0 para o
                            primeiro elemento, 1 para o segundo elemento e assim por diante. O índice ajuda a acessar e
                            manipular elementos específicos no vetor.</p>
    
                        <h4>3. Tamanho Fixo:</h4>
                        <p>Os vetores em C# têm um tamanho fixo, o que significa que você precisa especificar o número de
                            elementos que o vetor conterá quando o criar. Após a criação, o tamanho não pode ser alterado.
                        </p>
    
                        <h4>4. Declaração e Inicialização:</h4>
                        <p>Para criar um vetor, você deve declará-lo e inicializá-lo. A declaração informa ao compilador o
                            tipo de dado que o vetor conterá, enquanto a inicialização define o tamanho e, opcionalmente,
                            atribui valores iniciais aos elementos.</p>
    
                        <h4>5. Acesso aos Elementos:</h4>
                        <p>Você pode acessar elementos individuais em um vetor usando seus índices. Por exemplo, se você
                            tiver um vetor de inteiros, pode acessar o terceiro elemento usando o índice 2: `vetor[2]`.</p>
    
                        <h4>6. Manipulação de Dados:</h4>
                        <p>Vetores permitem que você armazene, modifique e recupere dados de forma eficiente. Isso é útil
                            para lidar com coleções de dados, como listas de compras, notas de alunos ou informações de
                            contato.</p>
    
                        <h4>7. Laços de Repetição:</h4>
                        <p>Os vetores são frequentemente combinados com estruturas de repetição, como "for" ou "foreach",
                            para processar todos os elementos de um vetor de maneira iterativa.</p>
    
                        <p>Em resumo, vetores em C# são uma maneira de armazenar e manipular coleções de elementos do mesmo
                            tipo. Eles são especialmente úteis quando você precisa lidar com um grupo de dados relacionados
                            e deseja acessar ou modificar esses dados de forma eficiente. Portanto, da próxima vez que você
                            trabalhar com vetores em seu código, lembre-se de que eles são como um conjunto ordenado de
                            elementos, cada um acessado por um índice numérico.</p>
    
    
                        <iframe width="699" height="393" src="https://www.youtube.com/embed/utkQHvmmJ38"
                            title="Título do Vídeo 6" frameborder="0"
                            allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
                            allowfullscreen>
                        </iframe>
                    </div>
                </div>
            </div>

        
    </section>

    <script src="https://unpkg.com/ionicons@5.1.2/dist/ionicons.js"></script>
    <script src="assets/js/main.js"></script>
    <script src="assets/js/materias.js"></script>


    <!-- ===== IONICONS ===== -->
    <script src="https://unpkg.com/ionicons@5.1.2/dist/ionicons.js"></script>

    <!-- ===== MAIN JS ===== -->
    <script src="assets/js/main.js"></script>

    <!-- ===== BOOTSTRAP ===== -->
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@4.0.0/dist/js/bootstrap.min.js"
        integrity="sha384-JZR6Spejh4U02d8jOt6vLEHfe/JQGiRRSQQxSfFWpi1MquVdAyjUar5+76PVCmYl" crossorigin="anonymous">
        </script>

</body>

</html>

------------------ caixadesaida.html-------------------

<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <!-- ===== BOOTSTRAP ===== -->
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/css/bootstrap.min.css" rel="stylesheet"
        integrity="sha384-T3c6CoIi6uLrA9TneNEoa7RxnatzjcDSCmG1MXxSR1GAsXEV/Dwwykc2MPK8M2HN" crossorigin="anonymous">
    <!-- ===== CSS ===== -->
    <link rel="stylesheet" href="assets/css/styles.css">
    <!-- ===== ICON ===== -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.2/css/all.min.css"
        integrity="sha512-z3gLpd7yknf1YoNbCzqRKc4qyor8gaKU1qmn+CShxbuBusANI9QpRohGBreCFkKxLhei6S9CQXFEbbKuqLg0DA=="
        crossorigin="anonymous" referrerpolicy="no-referrer" />

    <script src="https://code.jquery.com/jquery-3.5.1.slim.min.js"></script>
    <script src="https://cdn.jsdelivr.net/npm/@popperjs/core@2.9.3/dist/umd/popper.min.js"></script>

    <title>PUC Minas - Programa de Monitoria</title>
</head>

<body id="body-pd">
    <div class="l-navbar" id="navbar">
        <nav class="nav">
            <div>
                <div class="nav__brand">
                    <ion-icon name="menu-outline" class="nav__toggle" id="nav-toggle"></ion-icon>
                    <a href="caixadesaida.html" class="nav__logo"><img id="logo" src="assets/img/logo.png"
                            width="15%"></a>
                </div>

                <div class="nav__list">
                    <a href="painel_aluno.html" class="nav__link active">
                        <ion-icon name="home-outline" class="nav__icon"></ion-icon>
                        <span class="nav__name">Painel de Controle</span>
                    </a>

                    <a href="mensagem.html" class="nav__link">
                        <ion-icon name="chatbubbles-outline" class="nav__icon"></ion-icon>
                        <span class="nav__name">Mensagem</span>
                    </a>

                    <a href="agenda.html" class="nav__link">
                        <ion-icon name="calendar-outline" class="nav__icon"></ion-icon>
                        <span class="nav__name">Calendario</span>
                    </a>

                    <a href="https://teams.microsoft.com/dl/launcher/launcher.html?url=teams&type=meetup-join&enableMobilePage=true&suppressPrompt=true&tenantId=14cbd5a7-ec94-46ba-b314-cc0fc972a161"
                        class="nav__link">
                        <ion-icon name="tv" class="nav__icon"></ion-icon>
                        <span class="nav__name">Teams</span>
                    </a>


                    <a href="ajuda.html" class="nav__link">
                        <ion-icon name="help-outline" class="nav__icon"></ion-icon>
                        <span class="nav__name">Ajuda</span>
                    </a>

                    <a href="config.html" class="nav__link">
                        <ion-icon name="settings-outline" class="nav__icon"></ion-icon>
                        <span class="nav__name">Configurações</span>
                    </a>
                </div>
            </div>



            <div>
                <img id="foto" src="assets/img/foto.png" width="12%">
            </div>

            <a href="login.html" class="nav__link">
                <ion-icon name="log-out-outline" class="nav__icon"></ion-icon>
                <span class="nav__name">Sair</span>
            </a>
        </nav>
    </div>

    <section class="container-fluid">
        <div class="row">
            <div class="col-md-10">
                <div class="border-bottom" class="titulo">
                    <h1>Caixa de Saída</h1>
                </div>
            </div>
            <div class="col-2">
                <div>
                    <a href="login.html">
                        <button type="button" class="btn btn-dark"><i class="fa-solid fa-right-from-bracket"></i>
                            Sair</button>
                    </a>
                </div>
            </div>
        </div>

        <div class="row">
            <div class="col-md-2 pt-2">
                <link href="https://maxcdn.bootstrapcdn.com/font-awesome/4.3.0/css/font-awesome.min.css"
                    rel="stylesheet">
                <button type="button" class="btn btn-primary" data-bs-toggle="modal" data-bs-target="#modal1">
                    Enviar Mensagem
                </button>
                <hr>
                <div>
                    <ul>
                        <li class="header"><strong>Pastas</strong></li>
                        <li><a href="mensagem.html"><i class="fa fa-envelope"></i> Caixa de Entrada</a></li>
                        <li><a href="caixadesaida.html"><i class="fa fa-envelope-o"></i> Caixa de Saída</a></li>
                        <li><a href="importantes.html"><i class="fa fa-bookmark"></i> Importantes</a></li>
                        <li><a href="Lixeira.html"><i class="fa fa-pencil-square-o"></i> Lixeira</a></li>
                    </ul>
                </div>
            </div>

            <!-- BEGIN INBOX CONTENT -->
            <div class="col-md-9">
                <div class="row">
                    <div class="col-sm-6">
                        <label style="margin-right: 8px;" class="">
                            <div class="icheckbox_square-blue" style="position: relative;"><input type="checkbox"
                                    id="check-all" class="icheck"
                                    style="position: absolute; top: -20%; left: -20%; display: block; width: 140%; height: 140%; margin: 0px; padding: 0px; border: 0px; opacity: 0; background: rgb(255, 255, 255);"><ins
                                    class="iCheck-helper"
                                    style="position: absolute; top: -20%; left: -20%; display: block; width: 140%; height: 140%; margin: 0px; padding: 0px; border: 0px; opacity: 0; background: rgb(255, 255, 255);"></ins>
                            </div>
                        </label>

                        <div class="btn-group pt-4">
                            <button type="button" class="btn btn-default dropdown-toggle" data-toggle="dropdown">
                                Filtro <span class="caret"></span>
                            </button>
                            <ul class="dropdown-menu" role="menu">
                                <li><a href="#">Mark as read</a></li>
                                <li><a href="#">Mark as unread</a></li>
                                <li><a href="#">Mark as important</a></li>
                                <li><a href="#">Delete</a></li>
                            </ul>
                        </div>
                    </div>

                    <div class="col-md-6 search-form pt-2 pb-2 ">
                        <form action="#" class="text-right">
                            <div class="input-group">
                                <form class="d-flex" role="search">
                                    <input class="form-control me-2" type="search" placeholder="Pesquisar"
                                        aria-label="Search" id="searchInput">
                                    <button class="btn btn-outline-success" type="submit">Pesquisar</button>
                                </form>

                        </form>

                    </div>

                </div>

                <div class="padding"></div>
                <div class="text-danger mx-2">
                    <h6>Falha na entrega. Até que o e-mail seja totalmente entregue, ele permanecerá na Caixa de saída.
                    </h6>
                </div>
                <div class="table-responsive ">
                    <table class="table">
                        <tbody>
                            <tr id="message1">
                                <td class="action"><input type="checkbox" /> </td>
                                <td class="action"><i class="fa fa-bookmark-o"></i></td>
                                <td class="name text-danger"> [Não Enviada] <a href="#" data-bs-toggle="modal"
                                        data-bs-target="#modal2"> Clenilson
                                        Junior</a></td>
                                <td class="subject"><a href="#" data-bs-toggle="modal" data-bs-target="#modal2"> Olá,
                                        Clenilson
                                        claro que te ajudo com switch em C# </a></td>
                                <td class="time">08:30 PM</td>
                            </tr>
                            <tr id="message2">
                                <td class="action"><input type="checkbox" /></td>
                                <td class="action"><i class="fa fa-bookmark"></i></td>
                                <td class="name text-danger"> [Não Enviada]<a href="#" data-bs-toggle="modal"
                                        data-bs-target="#"> Gabriel Alvez</a>
                                </td>
                                <td class="subject"><a href="#" data-bs-toggle="modal" data-bs-target="#">
                                        Boa tarde, te ajudo sim com vetor em C# </a></td>
                                <td class="time">15:30 PM</td>
                            </tr>
                            <tr id="message3" class="read">
                                <td class="action"><input type="checkbox" /></td>
                                <td class="action"><i class="fa fa-bookmark"></i></td>
                                <td class="name text-danger"> [Não Enviada] <a href="#"> Tiago Barbacena</a></td>
                                <td class="subject"><a href="#">Boa noite, com certeza posso te ajudar com JAVASCRIPT
                                    </a></td>
                                <td class="time">18:30 PM</td>
                            </tr>
                            <tr id="message4">
                                <td class="action"><input type="checkbox" /></td>
                                <td class="action"><i class="fa fa-bookmark-o"></i></td>
                                <td class="name text-danger"> [Não Enviada]<a href="#"> Gabriela Martins</a></td>
                                <td class="subject"><a href="#">Bom dia, me envie sua dúvida na matéria ... </a></td>
                                <td class="time">07:30 PM</td>
                            </tr>
                            <tr id="message5" class="read">
                                <td class="action"><input type="checkbox" /></td>
                                <td class="action"><i class="fa fa-bookmark-o"></i></td>
                                <td class="name text-danger"> [Não Enviada]<a href="#"> Matheus Santiago</a></td>
                                <td class="subject"><a href="#">Ola, me mande o exercício que precisa de ajuda..</a>
                                </td>
                                <td class="time">08:30 PM</td>
                            </tr>

                        </tbody>
                    </table>
                </div>

                <nav>
                    <ul class="pagination">
                        <li class="page-item">
                            <a class="page-link" href="#">Voltar</a>
                        </li>
                        <li class="page-item"><a class="page-link" href="#">1</a></li>
                        <li class="page-item" aria-current="page">
                            <a class="page-link" href="#">2</a>
                        </li>
                        <li class="page-item"><a class="page-link" href="#">3</a></li>
                        <li class="page-item">
                            <a class="page-link" href="#">Proxima</a>
                        </li>
                    </ul>
                </nav>

                <script>
                    document.addEventListener('DOMContentLoaded', function () {
                        // Dados das mensagens
                        var messages = [
                            { id: 'message1', sender: 'Clenilson Junior', subject: 'Olá, Clenilson, claro que te ajudo com switch em C#', time: '08:30 PM' },
                            { id: 'message2', sender: 'Gabriel Alvez', subject: 'Boa tarde, te ajudo sim com vetor em C#', time: '15:30 PM' },
                            { id: 'message3', sender: 'Tiago Barbacena', subject: 'Boa noite, com certeza posso te ajudar com JAVASCRIPT', time: '18:30 PM' },
                            { id: 'message4', sender: 'Gabriela Martins', subject: 'Bom dia, me envie sua dúvida na matéria ...', time: '07:30 PM' },
                            { id: 'message5', sender: 'Matheus Santiago', subject: 'Ola, me mande o exercício que precisa de ajuda..', time: '08:30 PM' }
                            // Adicione mais mensagens conforme necessário
                        ];

                        // Função para exibir mensagens na tabela
                        function showMessages(page) {
                            var pageSize = 2; // Quantidade de mensagens por página
                            var start = (page - 1) * pageSize;
                            var end = start + pageSize;
                            var messagesToShow = messages.slice(start, end);

                            var tableBody = document.querySelector('.table tbody');
                            tableBody.innerHTML = ''; // Limpa o conteúdo atual da tabela

                            messagesToShow.forEach(function (message) {
                                var row = document.createElement('tr');
                                row.id = message.id;
                                row.innerHTML = `
                                    <td class="action"><input type="checkbox" /></td>
                                    <td class="action"><i class="fa fa-bookmark-o"></i></td>
                                    <td class="name text-danger"> [Não Enviada] <a href="#" data-bs-toggle="modal" data-bs-target="#modal2">${message.sender}</a></td>
                                    <td class="subject"><a href="#" data-bs-toggle="modal" data-bs-target="#modal2">${message.subject}</a></td>
                                    <td class="time">${message.time}</td>
                                `;
                                tableBody.appendChild(row);
                            });
                        }

                        // Função para navegar entre páginas
                        function navigatePage(action) {
                            var currentPage = parseInt(document.querySelector('.pagination li.active a').innerText);
                            var totalPages = Math.ceil(messages.length / 2); // 2 mensagens por página

                            if (action === 'prev' && currentPage > 1) {
                                showMessages(currentPage - 1);
                            } else if (action === 'next' && currentPage < totalPages) {
                                showMessages(currentPage + 1);
                            }
                        }

                        // Inicializa a página
                        showMessages(1);

                        // Adiciona eventos aos botões de páginação
                        document.querySelectorAll('.pagination a').forEach(function (pageLink) {
                            pageLink.addEventListener('click', function (event) {
                                event.preventDefault();
                                showMessages(parseInt(this.innerText));
                                document.querySelectorAll('.pagination li').forEach(function (li) {
                                    li.classList.remove('active');
                                });
                                this.parentElement.classList.add('active');
                            });
                        });

                        // Adiciona eventos aos botões de "Voltar" e "Próxima"
                        document.querySelector('.pagination li.prev a').addEventListener('click', function (event) {
                            event.preventDefault();
                            navigatePage('prev');
                        });

                        document.querySelector('.pagination li.next a').addEventListener('click', function (event) {
                            event.preventDefault();
                            navigatePage('next');
                        });
                    });
                </script>
                <!-- END INBOX CONTENT -->

                <script>
                    $(document).ready(function () {
                        $('#searchInput').on('input', function () {
                            var searchTerm = $(this).val().toLowerCase();

                            $('tbody tr').each(function () {
                                var name = $(this).find('.name a').text().toLowerCase();
                                var subject = $(this).find('.subject a').text().toLowerCase();

                                var match = name.includes(searchTerm) || subject.includes(searchTerm);

                                $(this).toggle(match);
                            });
                        });
                    });
                </script>
            </div>
        </div>
        </div>

        <!-- Modal 1 -->
        <div class="modal fade" id="modal1" tabindex="-1" aria-labelledby="exampleModalLabel" aria-hidden="true">
            <div class="modal-dialog">
                <div class="modal-content">
                    <div class="modal-header">
                        <h1 class="modal-title fs-5" id="exampleModalLabel">Nova mensagem</h1>
                        <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
                    </div>
                    <div class="modal-body">
                        <main>
                            <div class="panel-body contacts">
                                <button type="button" class="btn btn-primary" data-bs-toggle="modal"
                                    data-bs-target="#modal3"><i class="fa-solid fa-address-book"></i>
                                    Contatos
                                </button>
                            </div>
                            <form>
                                <div class="form-row mb-3">
                                    <label for="to" class="col-2 col-sm-1 col-form-label">Para:</label>
                                    <div class="col-10 col-sm-11">
                                        <input type="email" class="form-control" id="to" placeholder="email">
                                    </div>
                                </div>
                                <div class="form-row mb-3">
                                    <label for="cc" class="col-2 col-sm-1 col-form-label">Assunto:</label>
                                    <div class="col-10 col-sm-11">
                                        <input type="email" class="form-control" id="cc" placeholder="assunto">
                                    </div>
                                </div>

                                <div class="form-row mb-3">
                                    <label for="cc" class="col-2 col-sm-1 col-form-label">CC:</label>
                                    <div class="col-10 col-sm-11">
                                        <input type="email" class="form-control" id="cc" placeholder="copias">
                                    </div>
                                </div>

                            </form>
                            <div class="row">
                                <div class="col-sm-11 ml-auto">
                                    <div class="toolbar" role="toolbar">
                                        <div class="btn-group">
                                            <button type="button" class="btn btn-light">
                                                <span class="fa fa-bold"></span>
                                            </button>
                                            <button type="button" class="btn btn-light">
                                                <span class="fa fa-italic"></span>
                                            </button>
                                            <button type="button" class="btn btn-light">
                                                <span class="fa fa-underline"></span>
                                            </button>
                                        </div>

                                        <button type="button" class="btn btn-light">
                                            <span class="fa fa-trash-o"></span>
                                        </button>
                                        <button type="button" class="btn btn-light">
                                            <span class="fa fa-paperclip"></span>
                                        </button>
                                    </div>
                                    <div class="form-group mt-4">
                                        <textarea class="form-control" id="message" name="body" rows="12"
                                            placeholder="escrever"></textarea>
                                    </div>
                                    <div class="form-group mt-4">
                                        <button type="submit" class="btn btn-danger"
                                            data-bs-dismiss="modal">Cancelar</button>
                                        <button type="submit" class="btn btn-success">Enviar</button>
                                    </div>
                                </div>
                            </div>
                        </main>
                    </div>
                    <div class="modal-footer">
                        <button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Fechar</button>
                    </div>
                </div>
            </div>


            <script>
                document.addEventListener('DOMContentLoaded', function () {
                    document.querySelector('#modal1 .btn-success').addEventListener('click', function () {
                        alert('Mensagem enviada com sucesso!');
                        $('#modal1').modal('hide');
                    });
                });
            </script>
        </div>
        <!-- Modal 1 FIM -->

        <!-- Modal 2 -->
        <div class="modal fade" id="modal2" tabindex="-1" aria-labelledby="exampleModalLabel" aria-hidden="true">
            <div class="modal-dialog">
                <div class="modal-content">
                    <div class="modal-header">
                        <h1 class="modal-title fs-5" id="exampleModalLabel">Caixa de saída</h1>
                        <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
                    </div>
                    <div class="modal-body">
                        <main>
                            <link href="https://maxcdn.bootstrapcdn.com/font-awesome/4.3.0/css/font-awesome.min.css"
                                rel="stylesheet">
                            <div class="container">
                                <div class="row inbox">
                                    <div class="col-md-3">
                                        <div class="panel panel-default">
                                            <div class="panel-body inbox-menu">
                                                <a href="#" data-bs-toggle="modal" data-bs-target="#modal1"
                                                    class="btn btn-danger btn-block">Enviar Mensagem </a>
                                                <ul>
                                                    <li>
                                                        <a href="mensagem.html"><i class="fa fa-inbox"></i> Caixa de
                                                            Entrada <span class="label label-danger"></span></a>
                                                    </li>
                                                    <li>
                                                        <a href="caixadesaida.html"><i class="fa fa-rocket"></i> Caixa
                                                            de Saída</a>
                                                    </li>
                                                    <li>
                                                        <a href="Lixeira.html"><i class="fa fa-trash-o"></i> Lixo</a>
                                                    </li>
                                                    <li>
                                                        <a href="importantes.html"><i class="fa fa-bookmark"></i>
                                                            Importantes<span class="label label-info"></span></a>
                                                    </li>
                                                    <li class="title">
                                                </ul>
                                            </div>
                                        </div>
                                        <div class="panel panel-default">
                                            <div class="panel-body contacts">
                                                <button type="button" class="btn btn-primary" data-bs-toggle="modal"
                                                    data-bs-target="#modal3"><i class="fa-solid fa-address-book"></i>
                                                    Contatos
                                                </button>
                                            </div>
                                        </div>
                                    </div><!--/.col-->
                                    <div class="col-md-9">
                                        <div class="panel panel-default">
                                            <div class="panel-body message">
                                                <span class="btn-group">

                                                    <button id="importantBtn" class="btn btn-default"><span
                                                            class="fa fa-bookmark-o"></span></button>
                                                </span>
                                                <span class="btn-group">
                                                    <button class="btn btn-default"><span
                                                            class="fa fa-mail-reply"></span></button>
                                                    <button class="btn btn-default"><span
                                                            class="fa fa-mail-reply-all"></span></button>
                                                    <button class="btn btn-default"><span
                                                            class="fa fa-mail-forward"></span></button>
                                                </span>
                                                <button id="trashBtn" class="btn btn-default"><span
                                                        class="fa fa-trash-o"></span></button>

                                                <div class="message-title">Dificuldade em Switch </div>
                                                <div class="header">
                                                    <img class="avatar"
                                                        src="https://bootdey.com/img/Content/avatar/avatar1.png">
                                                    <div class="from text-dark">
                                                        <span>Clenilson Junior</span>
                                                        clenilsonjunior@holeczek.pl
                                                    </div>
                                                    <div class="date"><span class="fa fa-paper-clip"></span> Today,
                                                        <b>3:47 PM</b>
                                                    </div>
                                                    <div class="menu"></div>
                                                </div>
                                                <div class="content">
                                                    <p>
                                                        Olá, mentor! Tenho enfrentado algumas dificuldades com a
                                                        programação em C#. Sinto que preciso de ajuda para entender
                                                        melhor os conceitos de switch. Será que você pode me orientar?
                                                    </p>
                                                    <blockquote>
                                                        <!---->
                                                    </blockquote>
                                                </div>
                                                <!--MONITOR-->
                                                <div class="header">
                                                    <img class="avatar"
                                                        src="https://bootdey.com/img/Content/avatar/avatar3.png">
                                                    <div class="from text-dark">
                                                        <span>(EU) Monitor</span>
                                                        monitorfulanodetal@holeczek.pl
                                                    </div>
                                                    <div class="date"><span class="fa fa-paper-clip"></span> Today,
                                                        <b>4:10 PM</b>
                                                    </div>
                                                    <div class="menu"></div>
                                                </div>
                                                <div class="content">
                                                    <p>
                                                        Olá, Clenilson claro que te ajudo com switch em C#, que tal
                                                        marcarmos uma aula no Teams? Ou prefere que conversemos por
                                                        mensagem?
                                                    </p>
                                                    <blockquote>
                                                        <!---->
                                                    </blockquote>
                                                </div>



                                                <div class="attachments">
                                                    <ul>
                                                        <li>
                                                            <span class="label label-danger">zip</span>
                                                            <b>bootstrap.zip</b> <i>(2,5MB)</i>
                                                            <span class="quickMenu">
                                                                <a href="#" class="fa fa-search"><i></i></a>
                                                                <a href="#" class="fa fa-share"><i></i></a>
                                                                <a href="#" class="fa fa-cloud-download"><i></i></a>
                                                            </span>
                                                        </li>
                                                        <li>
                                                            <span class="label label-info">txt</span> <b>readme.txt</b>
                                                            <i>(7KB)</i>
                                                            <span class="quickMenu">
                                                                <a href="#" class="fa fa-search"><i></i></a>
                                                                <a href="#" class="fa fa-share"><i></i></a>
                                                                <a href="#" class="fa fa-cloud-download"><i></i></a>
                                                            </span>
                                                        </li>
                                                        <li>
                                                            <span class="label label-success">xls</span>
                                                            <b>spreadsheet.xls</b> <i>(984KB)</i>
                                                            <span class="quickMenu">
                                                                <a href="#" class="fa fa-search"><i></i></a>
                                                                <a href="#" class="fa fa-share"><i></i></a>
                                                                <a href="#" class="fa fa-cloud-download"><i></i></a>
                                                            </span>
                                                        </li>
                                                    </ul>
                                                </div>
                                                <form method="post" action="">
                                                    <div class="form-group">
                                                        <textarea class="form-control" id="message" name="body"
                                                            rows="12" placeholder="escreva"></textarea>
                                                    </div>
                                                    <div class="form-group pt-2">
                                                        <button tabindex="3" type="submit"
                                                            class="btn btn-success">Responder</button>
                                                    </div>
                                                </form>
                                            </div>
                                        </div>
                                    </div><!--/.col-->
                                </div>
                            </div>
                        </main>
                    </div>
                    <div class="modal-footer">
                        <button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Fechar</button>
                    </div>
                </div>
            </div>

            <script>
                document.addEventListener('DOMContentLoaded', function () {
                    document.querySelector('#importantBtn').addEventListener('click', function () {

                        alert('Email marcado como importante.');

                        $('#modal2').modal('hide');
                    });
                });
            </script>

            <script>
                document.addEventListener('DOMContentLoaded', function () {
                    document.querySelector('#trashBtn').addEventListener('click', function () {

                        alert('Email movido para a Lixeira.');

                        $('#modal2').modal('hide');
                    });
                });
            </script>

            <script>
                document.addEventListener('DOMContentLoaded', function () {
                    document.querySelector('#modal2 .btn-success').addEventListener('click', function (event) {
                        event.preventDefault();

                        alert('Mensagem enviada com sucesso!');

                        $('#modal2').modal('hide');
                    });
                });
            </script>
        </div>
        <!-- Modal 2 FIM -->

        <!-- Modal 3 -->
        <div class="modal fade" id="modal3" tabindex="-1" aria-labelledby="exampleModalLabel" aria-hidden="true">
            <div class="modal-dialog">
                <div class="modal-content">
                    <div class="modal-header">
                        <h1 class="modal-title fs-5" id="exampleModalLabel">Contatos</h1>
                        <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
                    </div>
                    <div class="modal-body">
                        <div class="container">
                            <div class="row align-items-center">
                                <div class="row" id="respostaRequisicao"></div>

                                <script>
                                    document.addEventListener('DOMContentLoaded', function () {
                                        // URL da sua API para buscar os dados do contato (substitua pelo seu URL real)
                                        var apiUrl = 'https://db.samuelcorreia4.repl.co/usuarios';

                                        // Realiza a requisição à API usando o fetch
                                        fetch(apiUrl)
                                            .then(response => response.json())
                                            .then(data => {
                                                // Manipula os dados recebidos e preenche a div com a resposta da requisição

                                                // Seleciona a div de resposta
                                                var respostaDiv = document.getElementById('respostaRequisicao');

                                                // Loop através dos contatos e cria os elementos HTML
                                                data.forEach(contact => {
                                                    // Cria um novo elemento de card para cada contato
                                                    var cardElement = document.createElement('div');
                                                    cardElement.className = 'col-xl-3 col-sm-6';

                                                    cardElement.innerHTML = `
                                                <div class="card">
                                                    <div class="card-body">
                                                        <div class="d-flex align-items-center">
                                                            <div>
                                                                <img src="${contact.foto}" alt="" class="avatar-md rounded-circle img-thumbnail" />
                                                            </div>
                                                            <div class="flex-1 ms-3">
                                                                <h5 class="font-size-16 mb-1"><a href="#" class="text-dark">${contact.usuario}</a></h5>
                                                            </div>
                                                        </div>
                                                        <div class="mt-3 pt-1">
                                                            <p class="text-muted mb-0"><i class="mdi mdi-phone font-size-15 align-middle pe-2 text-primary"></i>${contact.telefone}</p>
                                                            <p class="text-muted mb-0 mt-2"><i class="mdi mdi-email font-size-15 align-middle pe-2 text-primary"></i>${contact.email}</p>
                                                        </div>
                                                        <div class="d-flex gap-2 pt-4">
                                                            <button type="button" class="btn btn-primary btn-sm w-50" onclick="selecionarContato('${contact.usuario}', '${contact.telefone}', '${contact.email}')" data-bs-dismiss="modal"><i class="bx bx-message-square-dots me-1"></i>Selecionar</button>
                                                        </div>
                                                    </div>
                                                </div>
                                            `;

                                                    // Adiciona o novo card à div de resposta
                                                    respostaDiv.appendChild(cardElement);
                                                });
                                            })
                                            .catch(error => console.error('Erro na requisição:', error));

                                        // Função para preencher o Modal 1 com as informações do contato selecionado
                                        window.selecionarContato = function (nome, telefone, email) {
                                            document.getElementById('to').value = email;
                                            document.getElementById('cc').value = '';  // Limpar o campo CC
                                            document.getElementById('message').value = `Olá ${nome},\n\n`;  // Mensagem inicial
                                            $('#modal1').modal('show');  // Exibir o Modal 1
                                        };
                                    });
                                </script>
                            </div>
                            <div class="modal-footer">
                                <button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Fechar</button>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>

    </section>



    <!-- ===== IONICONS ===== -->
    <script src="https://unpkg.com/ionicons@5.1.2/dist/ionicons.js"></script>

    <!-- ===== MAIN JS ===== -->
    <script src="assets/js/main.js"></script>

    <!-- ===== BOOTSTRAP ===== -->
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.bundle.min.js"
        integrity="sha384-C6RzsynM9kWDrMNeT87bh95OGNyZPhcTNXj1NW7RuBCsyN/o0jlpcV8Qyq46cDfL"
        crossorigin="anonymous"></script>
</body>

</html>
------------------ config.html-------------------
<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/css/bootstrap.min.css" rel="stylesheet"
    integrity="sha384-T3c6CoIi6uLrA9TneNEoa7RxnatzjcDSCmG1MXxSR1GAsXEV/Dwwykc2MPK8M2HN" crossorigin="anonymous">
  <!-- ===== CSS ===== -->
  <link rel="stylesheet" href="assets/css/styles.css">
  <!-- ===== ICON ===== -->
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.2/css/all.min.css"
  integrity="sha512-z3gLpd7yknf1YoNbCzqRKc4qyor8gaKU1qmn+CShxbuBusANI9QpRohGBreCFkKxLhei6S9CQXFEbbKuqLg0DA=="
  crossorigin="anonymous" referrerpolicy="no-referrer" />

  <title>PUC Minas - Programa de Monitoria</title>
</head>

<body id="body-pd">

  <body id="body-pd">
    <div class="l-navbar" id="navbar">
      <nav class="nav">
        <div>
          <div class="nav__brand">
            <ion-icon name="menu-outline" class="nav__toggle" id="nav-toggle"></ion-icon>
            <a href="config.html" class="nav__logo"><img id="logo" src="assets/img/logo.png"
                width="15%"></a>
          </div>

          <div class="nav__list">
            <a href="painel_aluno.html" class="nav__link active">
              <ion-icon name="home-outline" class="nav__icon"></ion-icon>
              <span class="nav__name">Painel de Controle</span>
            </a>

            <a href="mensagem.html" class="nav__link">
              <ion-icon name="chatbubbles-outline" class="nav__icon"></ion-icon>
              <span class="nav__name">Mensagem</span>
            </a>

            <a href="agenda.html" class="nav__link">
              <ion-icon name="calendar-outline" class="nav__icon"></ion-icon>
              <span class="nav__name">Calendario</span>
            </a>

            <a href="https://teams.microsoft.com/dl/launcher/launcher.html?url=teams&type=meetup-join&enableMobilePage=true&suppressPrompt=true&tenantId=14cbd5a7-ec94-46ba-b314-cc0fc972a161"
              class="nav__link">
              <ion-icon name="tv" class="nav__icon"></ion-icon>
              <span class="nav__name">Teams</span>
            </a>


            <a href="ajuda.html" class="nav__link">
              <ion-icon name="help-outline" class="nav__icon"></ion-icon>
              <span class="nav__name">Ajuda</span>
            </a>

            <a href="config.html" class="nav__link">
              <ion-icon name="settings-outline" class="nav__icon"></ion-icon>
              <span class="nav__name">Configurações</span>
            </a>
          </div>
        </div>


        <div>
          <img id="foto" src="assets/img/foto.png" width="12%">
        </div>
        <a href="login.html" class="nav__link">
          <ion-icon name="log-out-outline" class="nav__icon"></ion-icon>
          <span class="nav__name">Sair</span>
        </a>
      </nav>
    </div>
    <div class="background-img">
      <!--Muda foto perfil-->
      <div class="card-body change-image">
        <div class="d-flex align-items-start align-items-sm-center gap-4">
          <img src="assets/img/foto.png" alt="user-avatar" class="d-block rounded" height="100" width="100"
            id="uploadedAvatar" />
          <div class="button-wrapper">
            <label for="upload" class="btn btn-primary me-2 mb-4" tabindex="0">
              <span class="d-none d-sm-block">Carregar</span>
              <i class="bx bx-upload d-block d-sm-none"></i>
              <input type="file" id="upload" class="account-file-input" hidden accept="image/png, image/jpeg" />
            </label>
            <p class="text-muted mb-0">Formatos permitidos JPG, GIF ou PNG</p>
          </div>
        </div>
      </div>

      <div class="container">

        <form class="well form-horizontal config-form" action=" " method="post" id="contact_form">
          <fieldset>

            <!-- Form Name -->
            <legend>Informações Pessoais</legend>

            <!-- Text input-->

            <div class="form-group">
              <label class="col-md-4 control-label">Primeiro Nome</label>
              <div class="col-md-4 inputGroupContainer">
                <div class="input-group">
                  <span class="input-group-addon"><i class="glyphicon glyphicon-user"></i></span>
                  <input name="first_name" placeholder="Primeiro Nome" class="form-control" type="text">
                </div>
              </div>
            </div>

            <!-- Text input-->

            <div class="form-group">
              <label class="col-md-4 control-label">Último Nome</label>
              <div class="col-md-4 inputGroupContainer">
                <div class="input-group">
                  <span class="input-group-addon"><i class="glyphicon glyphicon-user"></i></span>
                  <input name="last_name" placeholder="Último Nome" class="form-control" type="text">
                </div>
              </div>
            </div>

            <!-- Text input-->
            <div class="form-group">
              <label class="col-md-4 control-label">E-Mail</label>
              <div class="col-md-4 inputGroupContainer">
                <div class="input-group">
                  <span class="input-group-addon"><i class="glyphicon glyphicon-envelope"></i></span>
                  <input name="email" placeholder="E-Mail" class="form-control" type="text">
                </div>
              </div>
            </div>


            <!-- Text input-->

            <div class="form-group">
              <label class="col-md-4 control-label">Telefone</label>
              <div class="col-md-4 inputGroupContainer">
                <div class="input-group">
                  <span class="input-group-addon"><i class="glyphicon glyphicon-earphone"></i></span>
                  <input name="phone" placeholder="(+55)" class="form-control" type="text">
                </div>
              </div>
            </div>

            <!-- Text input-->

            <div class="form-group">
              <label class="col-md-4 control-label">Endereço</label>
              <div class="col-md-4 inputGroupContainer">
                <div class="input-group">
                  <span class="input-group-addon"><i class="glyphicon glyphicon-home"></i></span>
                  <input name="address" placeholder="Endereço" class="form-control" type="text">
                </div>
              </div>
            </div>

            <!-- Text input-->

            <div class="form-group">
              <label class="col-md-4 control-label">Cidade</label>
              <div class="col-md-4 inputGroupContainer">
                <div class="input-group">
                  <span class="input-group-addon"><i class="glyphicon glyphicon-home"></i></span>
                  <input name="city" placeholder="Cidade" class="form-control" type="text">
                </div>
              </div>
            </div>
            <!-- Text input-->

            <div class="form-group">
              <label class="col-md-4 control-label">CEP</label>
              <div class="col-md-4 inputGroupContainer">
                <div class="input-group">
                  <span class="input-group-addon"><i class="glyphicon glyphicon-home"></i></span>
                  <input name="zip" placeholder="CEP" class="form-control" type="text">
                </div>
              </div>
            </div>
            <!-- Button -->
            <div class="form-group">
              <label class="col-md-4 control-label"></label>
              <div class="col-md-4">
                <button type="submit" class="btn btn-warning" onclick="exibirAlerta()"><i class="fa-regular fa-floppy-disk"></i> Salvar </button>
                    <a href="login.html">
                <button type="button" class="btn btn-dark"><i class="fa-solid fa-right-from-bracket"></i> Sair</button>
              </a>

              <script>
                function exibirAlerta() {
                  alert("Configurações salvas com sucesso");
                }
              </script>
              </div>
            </div>

          </fieldset>
        </form>
      </div>
    </div>
    <!-- /.container -->
    <!-- ===== IONICONS ===== -->
    <script src="https://unpkg.com/ionicons@5.1.2/dist/ionicons.js"></script>

    <!-- ===== MAIN JS ===== -->
    <script src="assets/js/main.js"></script>

    <!--Config_JS-->
    <script src="assets/js/config.js"></script>
    <!-- ===== BOOTSTRAP ===== -->
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.bundle.min.js"
      integrity="sha384-C6RzsynM9kWDrMNeT87bh95OGNyZPhcTNXj1NW7RuBCsyN/o0jlpcV8Qyq46cDfL"
      crossorigin="anonymous"></script>
    </div>
  </body>

</html>

------------------ IC_aluno.html-------------------

<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap@4.0.0/dist/css/bootstrap.min.css"
        integrity="sha384-Gn5384xqQ1aoWXA+058RXPxPg6fy4IWvTNh0E263XmFcJlSAwiGgFAW/dAiS6JXm" crossorigin="anonymous">

    <!-- ===== CSS ===== -->
    <link rel="stylesheet" href="assets/css/styles.css">
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap@4.0.0/dist/css/bootstrap.min.css">
    <title>Conteúdos da Matéria</title>
    <script src="https://code.jquery.com/jquery-3.6.0.min.js"></script>
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@4.0.0/dist/js/bootstrap.min.js"></script>
    <style>
        .card-body iframe {
            display: block;
            margin: 0 auto;
            width: 95%;
            /* Ajuste a largura conforme necessário */
        }
    </style>

    </style>
</head>

<body id="body-pd">
    <a href="painel_aluno.html" class="btn btn-primary">Voltar</a>
    <div class="l-navbar" id="navbar">
        <nav class="nav">
            <div>
                <div class="nav__brand">
                    <ion-icon name="menu-outline" class="nav__toggle" id="nav-toggle"></ion-icon>
                    <a href="painel_aluno.html" class="nav__logo"><img id="logo" src="assets/img/logo.png"
                            width="15%"></a>
                </div>

                <div class="nav__list">
                    <a href="painel_aluno.html" class="nav__link active">
                        <ion-icon name="home-outline" class="nav__icon"></ion-icon>
                        <span class="nav__name">Painel de Controle</span>
                    </a>

                    <a href="mensagem.html" class="nav__link">
                        <ion-icon name="chatbubbles-outline" class="nav__icon"></ion-icon>
                        <span class="nav__name">Mensagem</span>
                    </a>

                    <a href="agenda.html" class="nav__link">
                        <ion-icon name="calendar-outline" class="nav__icon"></ion-icon>
                        <span class="nav__name">Calendario</span>
                    </a>

                    <a href="https://teams.microsoft.com/dl/launcher/launcher.html?url=teams&type=meetup-join&enableMobilePage=true&suppressPrompt=true&tenantId=14cbd5a7-ec94-46ba-b314-cc0fc972a161"
                        class="nav__link">
                        <ion-icon name="tv" class="nav__icon"></ion-icon>
                        <span class="nav__name">Teams</span>
                    </a>


                    <a href="ajuda.html" class="nav__link">
                        <ion-icon name="help-outline" class="nav__icon"></ion-icon>
                        <span class="nav__name">Ajuda</span>
                    </a>

                    <a href="config.html" class="nav__link">
                        <ion-icon name="settings-outline" class="nav__icon"></ion-icon>
                        <span class="nav__name">Configurações</span>
                    </a>
                </div>
            </div>


            <div>
                <img id="foto" src="assets/img/foto.png" width="12%">
            </div>

            <a href="login.html" class="nav__link">
                <ion-icon name="log-out-outline" class="nav__icon"></ion-icon>
                <span class="nav__name">Sair</span>
            </a>
        </nav>
    </div>

    <section class="container-fluid">
        <div class="titulo">
            <h1>
                <h1>Conteúdos da Matéria - Introdução à Computação</h1>
            </h1>
        </div>

        <!-- Conteúdo 1 -->
        <div class="card">
            <div class="card-header" id="contentHeading1">
                <h2 class="mb-0">
                    <button class="btn btn-link" type="button" data-toggle="collapse" data-target="#contentCollapse1"
                        aria-expanded="true" aria-controls="contentCollapse1">
                        Semana 1 - Este curso é pra mim? <ion-icon name="arrow-forward-outline"></ion-icon>
                    </button>
                </h2>
            </div>
            <div id="contentCollapse1" class="collapse" aria-labelledby="contentHeading1"
                data-parent="#contentAccordion">
                <div class="card-body">
                    <h3>Escolhendo Entre Sistemas de Informação e Análise e Desenvolvimento de Sistemas: Este Curso é
                        Para Mim?</h3>

                    <p>Quando se trata de decidir qual curso universitário seguir, muitos alunos se deparam com a
                        pergunta crucial: "Este curso é para mim?" É uma questão fundamental, pois a escolha de uma
                        graduação é um compromisso significativo de tempo e recursos. Duas opções que frequentemente
                        competem pela atenção dos estudantes são Sistemas de Informação (SI) e Análise e Desenvolvimento
                        de Sistemas (ADS). Cada um desses cursos tem suas próprias características e atrativos únicos. A
                        escolha entre eles dependerá de seus interesses, habilidades e metas de carreira.</p>

                    <h4>Sistemas de Informação (SI):</h4>
                    <ul>
                        <li>O curso de Sistemas de Informação é uma ótima opção para quem deseja compreender a
                            interseção entre tecnologia da informação e negócios. Os estudantes de SI aprendem a
                            projetar, implementar e gerenciar sistemas de informações que atendam às necessidades das
                            organizações. Eles se concentram em aspectos como análise de sistemas, gerenciamento de
                            projetos, segurança da informação e análise de dados. Portanto, se você é apaixonado por
                            tecnologia, mas também está interessado em questões de negócios e administração, SI pode ser
                            o curso certo para você.</li>
                    </ul>

                    <h4>Análise e Desenvolvimento de Sistemas (ADS):</h4>
                    <ul>
                        <li>Se a programação, o desenvolvimento de software e a resolução de problemas técnicos são o
                            que mais chamam sua atenção, o curso de Análise e Desenvolvimento de Sistemas pode ser a
                            escolha perfeita. O ADS é mais orientado para o desenvolvimento de software, onde os alunos
                            aprendem várias linguagens de programação, design de aplicativos e desenvolvimento de
                            sistemas. Os graduados em ADS geralmente se tornam programadores, desenvolvedores de
                            software ou engenheiros de software, trabalhando na criação de aplicativos e sistemas de
                            software inovadores.</li>
                    </ul>

                    <h3>Então, como decidir qual é o melhor para você?</h3>
                    <ul>
                        <li><strong>Interesses pessoais:</strong> Avalie seus interesses. Se você gosta de tecnologia e
                            se interessa por aspectos de negócios, SI pode ser uma ótima opção. Se você é um comunicador
                            eficaz e se interessa pela aplicação de soluções tecnológicas em ambientes de negócios, SI é
                            uma escolha sólida. Por outro lado, se você tem habilidades sólidas em programação e
                            resolução de problemas, o ADS pode ser a escolha natural.</li>
                        <li><strong>Habilidades e aptidões:</strong> Considere suas habilidades técnicas. Se você é um
                            entusiasta da programação e adora criar software, ADS pode ser mais adequado.</li>
                        <li><strong>Metas de carreira:</strong> Pergunte a si mesmo onde você vê sua carreira daqui a
                            cinco ou dez anos. Ambos os cursos oferecem oportunidades de carreira emocionantes, mas em
                            áreas diferentes. Se você deseja se tornar um analista de sistemas, consultor de TI ou
                            gerente de projeto, SI é uma opção. Para se tornar um desenvolvedor de software, engenheiro
                            de software ou arquiteto de soluções, ADS pode ser a escolha certa.</li>
                    </ul>

                    <p>Lembre-se de que a escolha do curso não é uma decisão definitiva e permanente. Muitos estudantes
                        eventualmente encontram maneiras de combinar elementos de ambos os campos em suas carreiras. O
                        importante é que você escolha um curso que o mantenha envolvido e motivado. Portanto, a resposta
                        para a pergunta "Este curso é para mim?" depende de suas paixões, objetivos e habilidades. Ambos
                        SI e ADS oferecem oportunidades empolgantes, e a escolha está em suas mãos.</p>

                    <p>Assista ao vídeo abaixo para obter mais informações sobre os cursos de Sistemas de Informação e
                        Análise e Desenvolvimento de Sistemas:</p>

                    <iframe width="699" height="393" src="https://www.youtube.com/embed/57wyfS560Uk"
                        title="Será que este curso é para mim? - @Curso em Vídeo HTML5 e CSS3" frameborder="0"
                        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
                        allowfullscreen></iframe>
                </div>
            </div>
        </div>
        <!-- Conteúdo 2 -->
        <div class="card">
            <div class="card-header" id="contentHeading2">
                <h2 class="mb-0">
                    <button class="btn btn-link" type="button" data-toggle="collapse" data-target="#contentCollapse2"
                        aria-expanded="true" aria-controls="contentCollapse2">
                        Semana 2 - De Onde Vem a Internet <ion-icon name="arrow-forward-outline"></ion-icon>
                    </button>
                </h2>
            </div>
            <div id="contentCollapse2" class="collapse" aria-labelledby="contentHeading2"
                data-parent="#contentAccordion">
                <div class="card-body">
                    <h3>De Onde Vem a Internet: Uma Explicação Simplificada</h3>
                    <p>A internet é uma parte essencial de nossas vidas diárias, mas você já parou para pensar de onde
                        ela realmente vem? Vamos dar uma olhada em uma explicação simplificada sobre a origem da
                        internet.</p>

                    <h4>1. Bits e Bytes:</h4>
                    <p>A internet é basicamente um gigantesco sistema de comunicação digital. Tudo começa com
                        informações digitais, representadas por "bits" (0s e 1s). Esses bits são como os tijolos com os
                        quais a internet é construída.</p>

                    <h4>2. Computadores e Servidores:</h4>
                    <p>Os computadores são como postos de troca de informações na internet. Eles armazenam sites da web,
                        enviam e recebem e-mails, hospedam mídia e muito mais. Esses computadores são chamados de
                        "servidores", e estão localizados em diferentes partes do mundo.</p>

                    <h4>3. Conexões de Rede:</h4>
                    <p>Para permitir que os computadores em todo o mundo se comuniquem, eles precisam estar conectados.
                        Isso é feito por meio de uma rede de computadores, que inclui cabos de fibra ótica, satélites,
                        cabos submarinos e até mesmo redes sem fio.</p>

                    <h4>4. Protocolos e Roteadores:</h4>
                    <p>A internet tem regras e padrões de comunicação chamados "protocolos". Eles garantem que os dados
                        sejam enviados e recebidos corretamente. Os "roteadores" são dispositivos que ajudam a
                        encaminhar os dados na direção certa, como uma espécie de carteiro da internet.</p>

                    <h4>5. O Papel dos Provedores de Internet:</h4>
                    <p>Provedores de Internet (ISPs) são empresas que fornecem acesso à internet para os usuários. Eles
                        atuam como uma ponte entre você e a vasta rede de servidores e computadores. Quando você
                        contrata um serviço de internet, seu provedor de internet ajuda a conectar seu dispositivo à
                        rede global.</p>

                    <h4>6. A World Wide Web (WWW):</h4>
                    <p>A World Wide Web é uma parte da internet que a maioria de nós usa diariamente. É uma coleção de
                        sites, páginas da web e recursos interconectados. Você acessa a web usando um navegador, como o
                        Chrome, o Firefox ou o Safari.</p>

                    <h4>7. Busca e Navegação:</h4>
                    <p>Para acessar informações na internet, você usa um mecanismo de busca, digita um endereço da web
                        ou segue links. Os servidores da web fornecem as páginas e informações que você solicita.</p>

                    <h4>8. Dados em Movimento:</h4>
                    <p>Quando você envia um e-mail, assiste a um vídeo ou faz uma chamada de vídeo, seus dados são
                        divididos em pacotes, enviados pela internet e, em seguida, recompostos em seu destino.</p>

                    <h4>9. Segurança e Privacidade:</h4>
                    <p>Manter a internet segura envolve criptografia e protocolos de segurança. É importante tomar
                        medidas para proteger sua privacidade online.</p>

                    <p>Em resumo, a internet é uma rede global que interconecta computadores, servidores e dispositivos
                        por meio de redes de comunicação. É uma rede de informações digitais que nos permite
                        compartilhar, aprender e explorar o mundo. Portanto, da próxima vez que você se perguntar de
                        onde vem a internet, lembre-se de que ela é formada por bits, cabos, servidores, protocolos e
                        provedores de internet, tudo trabalhando juntos para nos manter conectados.</p>

                    <iframe width="699" height="393" src="https://www.youtube.com/embed/F74GKCLXUWM"
                        title="Como a Internet chega na minha casa? - @Curso em Vídeo HTML5 e CSS3" frameborder="0"
                        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
                        allowfullscreen>
                    </iframe>
                </div>
            </div>
        </div>

        <!-- Conteudo 3 -->
        <div class="card">
            <div class="card-header" id="contentHeading3">
                <h2 class="mb-0">
                    <button class="btn btn-link" type="button" data-toggle="collapse" data-target="#contentCollapse3"
                        aria-expanded="true" aria-controls="contentCollapse3">
                        Semana 3 - HTML, CSS e JavaScript <ion-icon name="arrow-forward-outline"></ion-icon>
                    </button>
                </h2>
            </div>
            <div id="contentCollapse3" class="collapse" aria-labelledby="contentHeading3"
                data-parent="#contentAccordion">
                <div class="card-body">
                    <h3>Entendendo HTML, CSS e JavaScript</h3>
                    <p>O mundo da programação na web é impulsionado por três tecnologias essenciais: HTML, CSS e
                        JavaScript. Cada uma delas desempenha um papel fundamental na construção e no funcionamento dos
                        sites que você visita diariamente.</p>

                    <h4>HTML (Hypertext Markup Language)</h4>
                    <p>O HTML é a espinha dorsal de qualquer página da web. Ele fornece a estrutura e o conteúdo de uma
                        página, incluindo textos, imagens, links e outros elementos. O HTML é como a fundação de uma
                        casa, determinando a disposição dos elementos na página.</p>

                    <h4>CSS (Cascading Style Sheets)</h4>
                    <p>O CSS é responsável pela aparência e pelo design de uma página da web. Ele permite a estilização
                        de elementos HTML, como cores, fontes, espaçamentos e posicionamento. O CSS é como a pintura e a
                        decoração de uma casa, dando vida à estrutura HTML.</p>

                    <h4>JavaScript</h4>
                    <p>O JavaScript é a linguagem de programação que traz interatividade e dinamismo para uma página da
                        web. Com JavaScript, você pode criar funcionalidades como formulários interativos, galerias de
                        imagens deslizantes e muito mais. É como a eletricidade que faz os aparelhos em uma casa
                        funcionarem.</p>

                    <p>Em resumo, HTML cria a estrutura, CSS faz o design e JavaScript adiciona interatividade. Essas
                        tecnologias trabalham juntas para criar a experiência de navegação na web que você conhece. Ao
                        aprender essas três linguagens, você pode se tornar um construtor de sites habilidoso.</p>

                    <iframe width="699" height="393" src="https://www.youtube.com/embed/B4FU3NFRTDw"
                        title="A diferença entre HTML, CSS e JavaScript - @Curso em Vídeo HTML5 e CSS3" frameborder="0"
                        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
                        allowfullscreen>
                    </iframe>
                </div>
            </div>
        </div>

        <!-- Conteúdo 4 -->
        <div class="card">
            <div class="card-header" id="contentHeading4">
                <h2 class="mb-0">
                    <button class="btn btn-link" type="button" data-toggle="collapse" data-target="#contentCollapse4"
                        aria-expanded="true" aria-controls="contentCollapse4">
                        Semana 4 - Front-end, Back-end e Full Stack <ion-icon name="arrow-forward-outline"></ion-icon>
                    </button>
                </h2>
            </div>
            <div id="contentCollapse4" class="collapse" aria-labelledby="contentHeading4"
                data-parent="#contentAccordion">
                <div class="card-body">
                    <h3>Entendendo Front-end, Back-end e Full Stack</h3>
                    <p>Quando se trata de desenvolvimento web, existem três principais áreas de foco: Front-end,
                        Back-end e Full Stack. Cada uma dessas áreas descreve diferentes aspectos do desenvolvimento de
                        um site ou aplicativo.</p>

                    <h4>Front-end</h4>
                    <p>Front-end refere-se à parte de um site ou aplicativo que os usuários veem e interagem
                        diretamente. Isso inclui o layout, design, botões, menus e qualquer elemento com o qual os
                        usuários interagem em seus navegadores. Os desenvolvedores Front-end usam HTML, CSS e JavaScript
                        para criar uma experiência atraente para os usuários.</p>

                    <h4>Back-end</h4>
                    <p>O Back-end lida com a parte não visível de um site ou aplicativo. Isso envolve o processamento de
                        dados, a lógica do servidor, o armazenamento de informações em bancos de dados e a comunicação
                        com o Front-end. Os desenvolvedores Back-end trabalham com tecnologias como bancos de dados,
                        servidores web e linguagens de programação, como PHP, Python e Node.js.</p>

                    <h4>Full Stack</h4>
                    <p>Os desenvolvedores Full Stack têm habilidades em ambas as áreas: Front-end e Back-end. Eles são
                        capazes de criar uma aplicação completa, desde a interface do usuário até o funcionamento dos
                        servidores e bancos de dados. Isso os torna versáteis e capazes de lidar com todos os aspectos
                        de um projeto de desenvolvimento web.</p>

                    <p>Escolher entre Front-end, Back-end ou Full Stack depende de seus interesses e objetivos de
                        carreira. Cada área desempenha um papel vital na construção da web que usamos todos os dias.</p>

                    <iframe width="699" height="393" src="https://www.youtube.com/embed/iSqf2iPqJNM"
                        title="Front-end, Back-end e Full stack - @Curso em Vídeo HTML5 e CSS3" frameborder="0"
                        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
                        allowfullscreen></iframe>
                </div>
            </div>
        </div>


        <!-- Conteúdo 5 -->
        <div class="card">
            <div class="card-header" id="contentHeading5">
                <h2 class="mb-0">
                    <button class="btn btn-link" type="button" data-toggle="collapse" data-target="#contentCollapse5"
                        aria-expanded="true" aria-controls="contentCollapse5">
                        Semana 5 - Frameworks e bibliotecas? Quais as diferenças? <ion-icon
                            name="arrow-forward-outline"></ion-icon>
                    </button>
                </h2>
            </div>
            <div id="contentCollapse5" class="collapse" aria-labelledby="contentHeading5"
                data-parent="#contentAccordion">
                <div class="card-body">

                    <h3>Entendendo Frameworks e Bibliotecas</h3>
                    <p>No desenvolvimento de software, duas categorias importantes a serem consideradas são Frameworks e
                        Bibliotecas, cada uma desempenhando um papel fundamental na simplificação e aprimoramento do
                        processo de desenvolvimento.</p>

                    <h4>Framework</h4>
                    <p>Um framework é uma estrutura de desenvolvimento completa que fornece diretrizes e estruturas para
                        a construção de um aplicativo ou sistema. Ele define a arquitetura, o fluxo de trabalho e os
                        padrões de desenvolvimento, acelerando significativamente o processo de criação de software. Os
                        desenvolvedores usam um framework como base e, em seguida, personalizam e estendem suas
                        funcionalidades para atender às necessidades específicas do projeto. Exemplos populares de
                        frameworks incluem Angular, React, Ruby on Rails e Django.</p>

                    <h4>Biblioteca</h4>
                    <p>Por outro lado, uma biblioteca é um conjunto de funções ou componentes reutilizáveis que os
                        desenvolvedores podem incorporar em seus projetos para realizar tarefas específicas. Ao
                        contrário de um framework, uma biblioteca não impõe uma estrutura rígida; em vez disso, os
                        desenvolvedores têm mais flexibilidade e controle sobre como usar a biblioteca em seu código. As
                        bibliotecas são úteis para tarefas comuns, como manipulação de dados, manipulação de DOM ou
                        interações com APIs. Exemplos de bibliotecas incluem jQuery, React (que também pode ser usado
                        como uma biblioteca) e NumPy. </P>

                    <iframe width="699" height="393" src="https://www.youtube.com/embed/dp0zB4n3MUs"
                        title="Título do Vídeo 5" frameborder="0"
                        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
                        allowfullscreen>
                    </iframe>
                </div>
            </div>
        </div>

        <!-- Conteúdo 6 -->
        <div class="card">
            <div class="card-header" id="contentHeading6">
                <h2 class="mb-0">
                    <button class="btn btn-link" type="button" data-toggle="collapse" data-target="#contentCollapse6"
                        aria-expanded="true" aria-controls="contentCollapse6">
                        Semana 6 - Entendendo APIs <ion-icon name="arrow-forward-outline"></ion-icon>
                    </button>
                </h2>
            </div>
            <div id="contentCollapse6" class="collapse" aria-labelledby="contentHeading6"
                data-parent="#contentAccordion">
                <div class="card-body">

                    <h3>APIs (Interfaces de Programação de Aplicativos)</h3>

                    <h4>Ampla Variedade de Aplicações</h4>
                    <p>As APIs podem ser usadas para uma ampla variedade de aplicações específicas, como acessar dados
                        de um serviço da web, interagir com redes sociais, realizar transações financeiras, integrar
                        serviços de terceiros em seu aplicativo ou site e muito mais. Elas oferecem uma maneira
                        eficiente de ampliar as funcionalidades do seu software, sem a necessidade de desenvolver tudo
                        do zero.</p>

                    <h4>Componentes-Chave: Endpoints</h4>
                    <p>As APIs geralmente consistem em endpoints, que são URLs específicas para acesso a recursos ou
                        funcionalidades. Os desenvolvedores podem fazer recomendações para esses endpoints usando
                        métodos padrão, como GET, POST, PUT e DELETE, para recuperar ou enviar dados. As respostas das
                        APIs geralmente são retornadas em formatos comuns </p>

                    <h4>Documentação Necessária</h4>
                    <p>Para facilitar o uso das APIs, elas geralmente vêm com informações detalhadas que descrevem como
                        usar os endpoints, as parâmetros necessários e as respostas específicas. Essa documentação é
                        essencial para os desenvolvedores entenderem como interagir com a API de forma eficaz e como
                        aproveitar ao máximo seus recursos.</p>

                    <h4>Autenticação e Segurança</h4>
                    <p>A segurança desempenha um papel crítico no uso de APIs. Muitas APIs requerem autenticação para
                        garantir que apenas usuários autorizados acessem os recursos. Isso pode ser feito por meio de
                        chaves de API, tokens de acesso ou outros métodos de autenticação. Além disso, as boas práticas
                        de segurança, como a proteção contra ataques de segurança, são essenciais ao trabalhar com APIs.
                    </p>
                    <h4>Versionamento</h4>
                    <p>À medida que as APIs evoluem, é comum que novas versões sejam lançadas. O versionamento é
                        importante para garantir a compatibilidade com os aplicativos existentes. Os desenvolvedores
                        precisam estar cientes das versões da API que estão usando e acompanhar as atualizações para
                        evitar interrupções no funcionamento de seus aplicativos.</p>

                    <iframe width="699" height="393" src="https://www.youtube.com/embed/vGuqKIRWosk"
                        title="Título do Vídeo 6" frameborder="0"
                        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
                        allowfullscreen>
                    </iframe>
                </div>
            </div>
        </div>


    </section>

    <script src="https://unpkg.com/ionicons@5.1.2/dist/ionicons.js"></script>
    <script src="assets/js/main.js"></script>
    <script src="assets/js/materias.js"></script>


    <!-- ===== IONICONS ===== -->
    <script src="https://unpkg.com/ionicons@5.1.2/dist/ionicons.js"></script>

    <!-- ===== MAIN JS ===== -->
    <script src="assets/js/main.js"></script>

    <!-- ===== BOOTSTRAP ===== -->
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@4.0.0/dist/js/bootstrap.min.js"
        integrity="sha384-JZR6Spejh4U02d8jOt6vLEHfe/JQGiRRSQQxSfFWpi1MquVdAyjUar5+76PVCmYl" crossorigin="anonymous">
        </script>

</body>

</html>

------------------ IC_Monitor.html-------------------
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap@4.0.0/dist/css/bootstrap.min.css"
        integrity="sha384-Gn5384xqQ1aoWXA+058RXPxPg6fy4IWvTNh0E263XmFcJlSAwiGgFAW/dAiS6JXm" crossorigin="anonymous">

    <!-- ===== CSS ===== -->
    <link rel="stylesheet" href="assets/css/styles.css">
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap@4.0.0/dist/css/bootstrap.min.css">
    <title>Conteúdos da Matéria</title>
    <script src="https://code.jquery.com/jquery-3.6.0.min.js"></script>
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@4.0.0/dist/js/bootstrap.min.js"></script>
  
<style>
     .edit-btn,
    .delete-btn {
        position: absolute;
        top: 5px;
        z-index: 999;
        padding: 0.2rem 0.4rem;
        font-size: 0.75rem;
    }

    .edit-btn ion-icon,
    .delete-btn ion-icon {
        font-size: 1rem;
    }

    .edit-btn {
        right: 40px; /* Distância da borda direita para o botão de edição */
    }

    .delete-btn {
        right: 5px; /* Distância da borda direita para o botão de exclusão */
    }

    .card-header {
        position: relative;
    }
</style>



</head>

<body id="body-pd">
    <a href="painel_monitor.html" class="btn btn-primary">Voltar</a>
    <div class="l-navbar" id="navbar">
        <nav class="nav">
            <div>
                <div class="nav__brand">
                    <ion-icon name="menu-outline" class="nav__toggle" id="nav-toggle"></ion-icon>
                    <a href="painel_monitor.html" class="nav__logo"><img id="logo" src="assets/img/logo.png"
                            width="15%"></a>
                </div>

                <div class="nav__list">
                    <a href="painel_monitor.html" class="nav__link active">
                        <ion-icon name="home-outline" class="nav__icon"></ion-icon>
                        <span class="nav__name">Painel de Controle</span>
                    </a>


                    <a href="mensagem.html" class="nav__link">
                        <ion-icon name="chatbubbles-outline" class="nav__icon"></ion-icon>
                        <span class="nav__name">Mensagem</span>
                    </a>

                    <a href="agenda.html" class="nav__link">
                        <ion-icon name="calendar-outline" class="nav__icon"></ion-icon>
                        <span class="nav__name">Calendario</span>
                    </a>

                    <a href="https://teams.microsoft.com/dl/launcher/launcher.html?url=teams&type=meetup-join&enableMobilePage=true&suppressPrompt=true&tenantId=14cbd5a7-ec94-46ba-b314-cc0fc972a161"
                        class="nav__link">
                        <ion-icon name="tv" class="nav__icon"></ion-icon>
                        <span class="nav__name">Teams</span>
                    </a>


                    <a href="ajuda.html" class="nav__link">
                        <ion-icon name="help-outline" class="nav__icon"></ion-icon>
                        <span class="nav__name">Ajuda</span>
                    </a>

                    <a href="config.html" class="nav__link">
                        <ion-icon name="settings-outline" class="nav__icon"></ion-icon>
                        <span class="nav__name">Configurações</span>
                    </a>
                </div>
            </div>


            <div>
                <img id="foto" src="assets/img/foto.png" width="15%">
            </div>

            <a href="login.html" class="nav__link">
                <ion-icon name="log-out-outline" class="nav__icon"></ion-icon>
                <span class="nav__name">Sair</span>
            </a>
        </nav>
    </div>

    <section class="container-fluid">
        <div class="titulo">
            <h1>
                <h1>Conteúdos da Matéria - Introdução à Computação</h1>
            </h1>
        </div>

        <!-- Conteúdo 1 -->
        <div class="card">
            <div class="card-header position-relative" id="contentHeading1">
                <button class="btn btn-primary edit-btn"><ion-icon name="create-outline"></ion-icon></button>
                <button class="btn btn-danger delete-btn"><ion-icon name="trash-outline"></ion-icon></button>
                <h2 class="mb-0">
                    <button class="btn btn-link collapsed" type="button" data-toggle="collapse"
                        data-target="#contentCollapse1" aria-expanded="false" aria-controls="contentCollapse1">
                        Semana 1 - Este curso é pra mim? <ion-icon name="arrow-forward-outline"></ion-icon>
                    </button>
                </h2>
            </div>
            <div id="contentCollapse1" class="collapse" aria-labelledby="contentHeading1"
                data-parent="#contentAccordion">
                <div class="card-body">
                    <h3>Escolhendo Entre Sistemas de Informação e Análise e Desenvolvimento de Sistemas: Este Curso é
                        Para Mim?</h3>

                    <p>Quando se trata de decidir qual curso universitário seguir, muitos alunos se deparam com a
                        pergunta crucial: "Este curso é para mim?" É uma questão fundamental, pois a escolha de uma
                        graduação é um compromisso significativo de tempo e recursos. Duas opções que frequentemente
                        competem pela atenção dos estudantes são Sistemas de Informação (SI) e Análise e Desenvolvimento
                        de Sistemas (ADS). Cada um desses cursos tem suas próprias características e atrativos únicos. A
                        escolha entre eles dependerá de seus interesses, habilidades e metas de carreira.</p>

                    <h4>Sistemas de Informação (SI):</h4>
                    <ul>
                        <li>O curso de Sistemas de Informação é uma ótima opção para quem deseja compreender a
                            interseção entre tecnologia da informação e negócios. Os estudantes de SI aprendem a
                            projetar, implementar e gerenciar sistemas de informações que atendam às necessidades das
                            organizações. Eles se concentram em aspectos como análise de sistemas, gerenciamento de
                            projetos, segurança da informação e análise de dados. Portanto, se você é apaixonado por
                            tecnologia, mas também está interessado em questões de negócios e administração, SI pode ser
                            o curso certo para você.</li>
                    </ul>

                    <h4>Análise e Desenvolvimento de Sistemas (ADS):</h4>
                    <ul>
                        <li>Se a programação, o desenvolvimento de software e a resolução de problemas técnicos são o
                            que mais chamam sua atenção, o curso de Análise e Desenvolvimento de Sistemas pode ser a
                            escolha perfeita. O ADS é mais orientado para o desenvolvimento de software, onde os alunos
                            aprendem várias linguagens de programação, design de aplicativos e desenvolvimento de
                            sistemas. Os graduados em ADS geralmente se tornam programadores, desenvolvedores de
                            software ou engenheiros de software, trabalhando na criação de aplicativos e sistemas de
                            software inovadores.</li>
                    </ul>

                    <h3>Então, como decidir qual é o melhor para você?</h3>
                    <ul>
                        <li><strong>Interesses pessoais:</strong> Avalie seus interesses. Se você gosta de tecnologia e
                            se interessa por aspectos de negócios, SI pode ser uma ótima opção. Se você é um comunicador
                            eficaz e se interessa pela aplicação de soluções tecnológicas em ambientes de negócios, SI é
                            uma escolha sólida. Por outro lado, se você tem habilidades sólidas em programação e
                            resolução de problemas, o ADS pode ser a escolha natural.</li>
                        <li><strong>Habilidades e aptidões:</strong> Considere suas habilidades técnicas. Se você é um
                            entusiasta da programação e adora criar software, ADS pode ser mais adequado.</li>
                        <li><strong>Metas de carreira:</strong> Pergunte a si mesmo onde você vê sua carreira daqui a
                            cinco ou dez anos. Ambos os cursos oferecem oportunidades de carreira emocionantes, mas em
                            áreas diferentes. Se você deseja se tornar um analista de sistemas, consultor de TI ou
                            gerente de projeto, SI é uma opção. Para se tornar um desenvolvedor de software, engenheiro
                            de software ou arquiteto de soluções, ADS pode ser a escolha certa.</li>
                    </ul>

                    <p>Lembre-se de que a escolha do curso não é uma decisão definitiva e permanente. Muitos estudantes
                        eventualmente encontram maneiras de combinar elementos de ambos os campos em suas carreiras. O
                        importante é que você escolha um curso que o mantenha envolvido e motivado. Portanto, a resposta
                        para a pergunta "Este curso é para mim?" depende de suas paixões, objetivos e habilidades. Ambos
                        SI e ADS oferecem oportunidades empolgantes, e a escolha está em suas mãos.</p>

                    <p>Assista ao vídeo abaixo para obter mais informações sobre os cursos de Sistemas de Informação e
                        Análise e Desenvolvimento de Sistemas:</p>

                    <iframe width="699" height="393" src="https://www.youtube.com/embed/57wyfS560Uk"
                        title="Será que este curso é para mim? - @Curso em Vídeo HTML5 e CSS3" frameborder="0"
                        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
                        allowfullscreen></iframe>
                </div>
            </div>
        </div>


        <!-- Conteúdo 2 -->
        <div class="card">
            <div class="card-header" id="contentHeading2">
                <h2 class="mb-0">
                    <div class="d-flex justify-content-center"> <!-- ou justify-content-center -->
                        <button class="btn btn-primary edit-btn"><ion-icon name="create-outline"></ion-icon></button>
                        <button class="btn btn-danger delete-btn"><ion-icon name="trash-outline"></ion-icon></button>
                    </div>
                    <button class="btn btn-link" type="button" data-toggle="collapse" data-target="#contentCollapse2"
                        aria-expanded="true" aria-controls="contentCollapse2">
                        Semana 2 - De Onde Vem a Internet <ion-icon name="arrow-forward-outline"></ion-icon>
                    </button>
                </h2>
            </div>
            <div id="contentCollapse2" class="collapse" aria-labelledby="contentHeading2"
                data-parent="#contentAccordion">
                <div class="card-body">
                    <h3>De Onde Vem a Internet: Uma Explicação Simplificada</h3>
                    <p>A internet é uma parte essencial de nossas vidas diárias, mas você já parou para pensar de onde
                        ela realmente vem? Vamos dar uma olhada em uma explicação simplificada sobre a origem da
                        internet.</p>

                    <h4>1. Bits e Bytes:</h4>
                    <p>A internet é basicamente um gigantesco sistema de comunicação digital. Tudo começa com
                        informações digitais, representadas por "bits" (0s e 1s). Esses bits são como os tijolos com os
                        quais a internet é construída.</p>

                    <h4>2. Computadores e Servidores:</h4>
                    <p>Os computadores são como postos de troca de informações na internet. Eles armazenam sites da web,
                        enviam e recebem e-mails, hospedam mídia e muito mais. Esses computadores são chamados de
                        "servidores", e estão localizados em diferentes partes do mundo.</p>

                    <h4>3. Conexões de Rede:</h4>
                    <p>Para permitir que os computadores em todo o mundo se comuniquem, eles precisam estar conectados.
                        Isso é feito por meio de uma rede de computadores, que inclui cabos de fibra ótica, satélites,
                        cabos submarinos e até mesmo redes sem fio.</p>

                    <h4>4. Protocolos e Roteadores:</h4>
                    <p>A internet tem regras e padrões de comunicação chamados "protocolos". Eles garantem que os dados
                        sejam enviados e recebidos corretamente. Os "roteadores" são dispositivos que ajudam a
                        encaminhar os dados na direção certa, como uma espécie de carteiro da internet.</p>

                    <h4>5. O Papel dos Provedores de Internet:</h4>
                    <p>Provedores de Internet (ISPs) são empresas que fornecem acesso à internet para os usuários. Eles
                        atuam como uma ponte entre você e a vasta rede de servidores e computadores. Quando você
                        contrata um serviço de internet, seu provedor de internet ajuda a conectar seu dispositivo à
                        rede global.</p>

                    <h4>6. A World Wide Web (WWW):</h4>
                    <p>A World Wide Web é uma parte da internet que a maioria de nós usa diariamente. É uma coleção de
                        sites, páginas da web e recursos interconectados. Você acessa a web usando um navegador, como o
                        Chrome, o Firefox ou o Safari.</p>

                    <h4>7. Busca e Navegação:</h4>
                    <p>Para acessar informações na internet, você usa um mecanismo de busca, digita um endereço da web
                        ou segue links. Os servidores da web fornecem as páginas e informações que você solicita.</p>

                    <h4>8. Dados em Movimento:</h4>
                    <p>Quando você envia um e-mail, assiste a um vídeo ou faz uma chamada de vídeo, seus dados são
                        divididos em pacotes, enviados pela internet e, em seguida, recompostos em seu destino.</p>

                    <h4>9. Segurança e Privacidade:</h4>
                    <p>Manter a internet segura envolve criptografia e protocolos de segurança. É importante tomar
                        medidas para proteger sua privacidade online.</p>

                    <p>Em resumo, a internet é uma rede global que interconecta computadores, servidores e dispositivos
                        por meio de redes de comunicação. É uma rede de informações digitais que nos permite
                        compartilhar, aprender e explorar o mundo. Portanto, da próxima vez que você se perguntar de
                        onde vem a internet, lembre-se de que ela é formada por bits, cabos, servidores, protocolos e
                        provedores de internet, tudo trabalhando juntos para nos manter conectados.</p>

                    <iframe width="699" height="393" src="https://www.youtube.com/embed/F74GKCLXUWM"
                        title="Como a Internet chega na minha casa? - @Curso em Vídeo HTML5 e CSS3" frameborder="0"
                        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
                        allowfullscreen>
                    </iframe>
                </div>
            </div>
        </div>

        <!-- Conteudo 3 -->
        <div class="card">
            <div class="card-header" id="contentHeading3">
                <div class="d-flex justify-content-center"> <!-- ou justify-content-center -->
                    <button class="btn btn-primary edit-btn"><ion-icon name="create-outline"></ion-icon></button>
                    <button class="btn btn-danger delete-btn"><ion-icon name="trash-outline"></ion-icon></button>
                </div>
                <h2 class="mb-0">
                    <button class="btn btn-link" type="button" data-toggle="collapse" data-target="#contentCollapse3"
                        aria-expanded="true" aria-controls="contentCollapse3">
                        Semana 3 - HTML, CSS e JavaScript <ion-icon name="arrow-forward-outline"></ion-icon>
                    </button>
                </h2>
            </div>
            <div id="contentCollapse3" class="collapse" aria-labelledby="contentHeading3"
                data-parent="#contentAccordion">
                <div class="card-body">
                    <h3>Entendendo HTML, CSS e JavaScript</h3>
                    <p>O mundo da programação na web é impulsionado por três tecnologias essenciais: HTML, CSS e
                        JavaScript. Cada uma delas desempenha um papel fundamental na construção e no funcionamento dos
                        sites que você visita diariamente.</p>

                    <h4>HTML (Hypertext Markup Language)</h4>
                    <p>O HTML é a espinha dorsal de qualquer página da web. Ele fornece a estrutura e o conteúdo de uma
                        página, incluindo textos, imagens, links e outros elementos. O HTML é como a fundação de uma
                        casa, determinando a disposição dos elementos na página.</p>

                    <h4>CSS (Cascading Style Sheets)</h4>
                    <p>O CSS é responsável pela aparência e pelo design de uma página da web. Ele permite a estilização
                        de elementos HTML, como cores, fontes, espaçamentos e posicionamento. O CSS é como a pintura e a
                        decoração de uma casa, dando vida à estrutura HTML.</p>

                    <h4>JavaScript</h4>
                    <p>O JavaScript é a linguagem de programação que traz interatividade e dinamismo para uma página da
                        web. Com JavaScript, você pode criar funcionalidades como formulários interativos, galerias de
                        imagens deslizantes e muito mais. É como a eletricidade que faz os aparelhos em uma casa
                        funcionarem.</p>

                    <p>Em resumo, HTML cria a estrutura, CSS faz o design e JavaScript adiciona interatividade. Essas
                        tecnologias trabalham juntas para criar a experiência de navegação na web que você conhece. Ao
                        aprender essas três linguagens, você pode se tornar um construtor de sites habilidoso.</p>

                    <iframe width="699" height="393" src="https://www.youtube.com/embed/B4FU3NFRTDw"
                        title="A diferença entre HTML, CSS e JavaScript - @Curso em Vídeo HTML5 e CSS3" frameborder="0"
                        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
                        allowfullscreen>
                    </iframe>
                </div>
            </div>
        </div>

        <!-- Conteúdo 4 -->
        <div class="card">
            <div class="card-header" id="contentHeading3">
                <div class="d-flex justify-content-center"> <!-- ou justify-content-center -->
                    <button class="btn btn-primary edit-btn"><ion-icon name="create-outline"></ion-icon></button>
                    <button class="btn btn-danger delete-btn"><ion-icon name="trash-outline"></ion-icon></button>
                </div>
                <h2 class="mb-0">
                    <button class="btn btn-link" type="button" data-toggle="collapse" data-target="#contentCollapse4"
                        aria-expanded="true" aria-controls="contentCollapse4">
                        Semana 4 - Front-end, Back-end e Full Stack <ion-icon name="arrow-forward-outline"></ion-icon>
                    </button>
                </h2>
            </div>
            <div id="contentCollapse4" class="collapse" aria-labelledby="contentHeading4"
                data-parent="#contentAccordion">
                <div class="card-body">
                    <h3>Entendendo Front-end, Back-end e Full Stack</h3>
                    <p>Quando se trata de desenvolvimento web, existem três principais áreas de foco: Front-end,
                        Back-end e Full Stack. Cada uma dessas áreas descreve diferentes aspectos do desenvolvimento de
                        um site ou aplicativo.</p>

                    <h4>Front-end</h4>
                    <p>Front-end refere-se à parte de um site ou aplicativo que os usuários veem e interagem
                        diretamente. Isso inclui o layout, design, botões, menus e qualquer elemento com o qual os
                        usuários interagem em seus navegadores. Os desenvolvedores Front-end usam HTML, CSS e JavaScript
                        para criar uma experiência atraente para os usuários.</p>

                    <h4>Back-end</h4>
                    <p>O Back-end lida com a parte não visível de um site ou aplicativo. Isso envolve o processamento de
                        dados, a lógica do servidor, o armazenamento de informações em bancos de dados e a comunicação
                        com o Front-end. Os desenvolvedores Back-end trabalham com tecnologias como bancos de dados,
                        servidores web e linguagens de programação, como PHP, Python e Node.js.</p>

                    <h4>Full Stack</h4>
                    <p>Os desenvolvedores Full Stack têm habilidades em ambas as áreas: Front-end e Back-end. Eles são
                        capazes de criar uma aplicação completa, desde a interface do usuário até o funcionamento dos
                        servidores e bancos de dados. Isso os torna versáteis e capazes de lidar com todos os aspectos
                        de um projeto de desenvolvimento web.</p>

                    <p>Escolher entre Front-end, Back-end ou Full Stack depende de seus interesses e objetivos de
                        carreira. Cada área desempenha um papel vital na construção da web que usamos todos os dias.</p>

                    <iframe width="699" height="393" src="https://www.youtube.com/embed/iSqf2iPqJNM"
                        title="Front-end, Back-end e Full stack - @Curso em Vídeo HTML5 e CSS3" frameborder="0"
                        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
                        allowfullscreen></iframe>
                </div>
            </div>
        </div>


        <!-- Conteúdo 5 -->
        <div class="card">
            <div class="card-header" id="contentHeading3">
                <div class="d-flex justify-content-center"> <!-- ou justify-content-center -->
                    <button class="btn btn-primary edit-btn"><ion-icon name="create-outline"></ion-icon></button>
                    <button class="btn btn-danger delete-btn"><ion-icon name="trash-outline"></ion-icon></button>
                </div>
                <h2 class="mb-0">
                    <button class="btn btn-link" type="button" data-toggle="collapse" data-target="#contentCollapse5"
                        aria-expanded="true" aria-controls="contentCollapse5">
                        Semana 5 - Frameworks e bibliotecas? Quais as diferenças? <ion-icon
                            name="arrow-forward-outline"></ion-icon>
                    </button>
                </h2>
            </div>
            <div id="contentCollapse5" class="collapse" aria-labelledby="contentHeading5"
                data-parent="#contentAccordion">
                <div class="card-body">

                    <h3>Entendendo Frameworks e Bibliotecas</h3>
                    <p>No desenvolvimento de software, duas categorias importantes a serem consideradas são Frameworks e
                        Bibliotecas, cada uma desempenhando um papel fundamental na simplificação e aprimoramento do
                        processo de desenvolvimento.</p>

                    <h4>Framework</h4>
                    <p>Um framework é uma estrutura de desenvolvimento completa que fornece diretrizes e estruturas para
                        a construção de um aplicativo ou sistema. Ele define a arquitetura, o fluxo de trabalho e os
                        padrões de desenvolvimento, acelerando significativamente o processo de criação de software. Os
                        desenvolvedores usam um framework como base e, em seguida, personalizam e estendem suas
                        funcionalidades para atender às necessidades específicas do projeto. Exemplos populares de
                        frameworks incluem Angular, React, Ruby on Rails e Django.</p>

                    <h4>Biblioteca</h4>
                    <p>Por outro lado, uma biblioteca é um conjunto de funções ou componentes reutilizáveis que os
                        desenvolvedores podem incorporar em seus projetos para realizar tarefas específicas. Ao
                        contrário de um framework, uma biblioteca não impõe uma estrutura rígida; em vez disso, os
                        desenvolvedores têm mais flexibilidade e controle sobre como usar a biblioteca em seu código. As
                        bibliotecas são úteis para tarefas comuns, como manipulação de dados, manipulação de DOM ou
                        interações com APIs. Exemplos de bibliotecas incluem jQuery, React (que também pode ser usado
                        como uma biblioteca) e NumPy. </P>

                    <iframe width="699" height="393" src="https://www.youtube.com/embed/dp0zB4n3MUs"
                        title="Título do Vídeo 5" frameborder="0"
                        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
                        allowfullscreen>
                    </iframe>
                </div>
            </div>
        </div>

        <!-- Conteúdo 6 -->
        <div class="card">
            <div class="card-header" id="contentHeading3">
                <div class="d-flex justify-content-center"> <!-- ou justify-content-center -->
                    <button class="btn btn-primary edit-btn"><ion-icon name="create-outline"></ion-icon></button>
                    <button class="btn btn-danger delete-btn"><ion-icon name="trash-outline"></ion-icon></button>
                </div>
                <h2 class="mb-0">
                    <button class="btn btn-link" type="button" data-toggle="collapse" data-target="#contentCollapse6"
                        aria-expanded="true" aria-controls="contentCollapse6">
                        Semana 6 - Entendendo APIs <ion-icon name="arrow-forward-outline"></ion-icon>
                    </button>
                </h2>
            </div>
            <div id="contentCollapse6" class="collapse" aria-labelledby="contentHeading6"
                data-parent="#contentAccordion">
                <div class="card-body">

                    <h3>APIs (Interfaces de Programação de Aplicativos)</h3>

                    <h4>Ampla Variedade de Aplicações</h4>
                    <p>As APIs podem ser usadas para uma ampla variedade de aplicações específicas, como acessar dados
                        de um serviço da web, interagir com redes sociais, realizar transações financeiras, integrar
                        serviços de terceiros em seu aplicativo ou site e muito mais. Elas oferecem uma maneira
                        eficiente de ampliar as funcionalidades do seu software, sem a necessidade de desenvolver tudo
                        do zero.</p>

                    <h4>Componentes-Chave: Endpoints</h4>
                    <p>As APIs geralmente consistem em endpoints, que são URLs específicas para acesso a recursos ou
                        funcionalidades. Os desenvolvedores podem fazer recomendações para esses endpoints usando
                        métodos padrão, como GET, POST, PUT e DELETE, para recuperar ou enviar dados. As respostas das
                        APIs geralmente são retornadas em formatos comuns </p>

                    <h4>Documentação Necessária</h4>
                    <p>Para facilitar o uso das APIs, elas geralmente vêm com informações detalhadas que descrevem como
                        usar os endpoints, as parâmetros necessários e as respostas específicas. Essa documentação é
                        essencial para os desenvolvedores entenderem como interagir com a API de forma eficaz e como
                        aproveitar ao máximo seus recursos.</p>

                    <h4>Autenticação e Segurança</h4>
                    <p>A segurança desempenha um papel crítico no uso de APIs. Muitas APIs requerem autenticação para
                        garantir que apenas usuários autorizados acessem os recursos. Isso pode ser feito por meio de
                        chaves de API, tokens de acesso ou outros métodos de autenticação. Além disso, as boas práticas
                        de segurança, como a proteção contra ataques de segurança, são essenciais ao trabalhar com APIs.
                    </p>
                    <h4>Versionamento</h4>
                    <p>À medida que as APIs evoluem, é comum que novas versões sejam lançadas. O versionamento é
                        importante para garantir a compatibilidade com os aplicativos existentes. Os desenvolvedores
                        precisam estar cientes das versões da API que estão usando e acompanhar as atualizações para
                        evitar interrupções no funcionamento de seus aplicativos.</p>

                    <iframe width="699" height="393" src="https://www.youtube.com/embed/vGuqKIRWosk"
                        title="Título do Vídeo 6" frameborder="0"
                        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
                        allowfullscreen>
                    </iframe>
                </div>
            </div>
        </div>


    </section>

    <script src="https://unpkg.com/ionicons@5.1.2/dist/ionicons.js"></script>
    <script src="assets/js/main.js"></script>
    <script src="assets/js/materias.js"></script>


    <!-- ===== IONICONS ===== -->
    <script src="https://unpkg.com/ionicons@5.1.2/dist/ionicons.js"></script>

    <!-- ===== MAIN JS ===== -->
    <script src="assets/js/main.js"></script>

    <!-- ===== BOOTSTRAP ===== -->
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@4.0.0/dist/js/bootstrap.min.js"
        integrity="sha384-JZR6Spejh4U02d8jOt6vLEHfe/JQGiRRSQQxSfFWpi1MquVdAyjUar5+76PVCmYl" crossorigin="anonymous">
        </script>

</body>

</html>

------------------ importantes.html-------------------

<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <!-- ===== BOOTSTRAP ===== -->
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/css/bootstrap.min.css" rel="stylesheet"
        integrity="sha384-T3c6CoIi6uLrA9TneNEoa7RxnatzjcDSCmG1MXxSR1GAsXEV/Dwwykc2MPK8M2HN" crossorigin="anonymous">
    <!-- ===== CSS ===== -->
    <link rel="stylesheet" href="assets/css/styles.css">
    <!-- ===== ICON ===== -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.2/css/all.min.css"
        integrity="sha512-z3gLpd7yknf1YoNbCzqRKc4qyor8gaKU1qmn+CShxbuBusANI9QpRohGBreCFkKxLhei6S9CQXFEbbKuqLg0DA=="
        crossorigin="anonymous" referrerpolicy="no-referrer" />

    <script src="https://code.jquery.com/jquery-3.5.1.slim.min.js"></script>
    <script src="https://cdn.jsdelivr.net/npm/@popperjs/core@2.9.3/dist/umd/popper.min.js"></script>

    <title>PUC Minas - Programa de Monitoria</title>
</head>

<body id="body-pd">
    <div class="l-navbar" id="navbar">
        <nav class="nav">
            <div>
                <div class="nav__brand">
                    <ion-icon name="menu-outline" class="nav__toggle" id="nav-toggle"></ion-icon>
                    <a href="importantes.html" class="nav__logo"><img id="logo" src="assets/img/logo.png"
                            width="15%"></a>
                </div>

                <div class="nav__list">
                    <a href="painel_aluno.html" class="nav__link active">
                        <ion-icon name="home-outline" class="nav__icon"></ion-icon>
                        <span class="nav__name">Painel de Controle</span>
                    </a>

                    <a href="mensagem.html" class="nav__link">
                        <ion-icon name="chatbubbles-outline" class="nav__icon"></ion-icon>
                        <span class="nav__name">Mensagem</span>
                    </a>

                    <a href="agenda.html" class="nav__link">
                        <ion-icon name="calendar-outline" class="nav__icon"></ion-icon>
                        <span class="nav__name">Calendario</span>
                    </a>

                    <a href="https://teams.microsoft.com/dl/launcher/launcher.html?url=teams&type=meetup-join&enableMobilePage=true&suppressPrompt=true&tenantId=14cbd5a7-ec94-46ba-b314-cc0fc972a161"
                        class="nav__link">
                        <ion-icon name="tv" class="nav__icon"></ion-icon>
                        <span class="nav__name">Teams</span>
                    </a>


                    <a href="ajuda.html" class="nav__link">
                        <ion-icon name="help-outline" class="nav__icon"></ion-icon>
                        <span class="nav__name">Ajuda</span>
                    </a>

                    <a href="config.html" class="nav__link">
                        <ion-icon name="settings-outline" class="nav__icon"></ion-icon>
                        <span class="nav__name">Configurações</span>
                    </a>
                </div>
            </div>



            <div>
                <img id="foto" src="assets/img/foto.png" width="12%">
            </div>

            <a href="login.html" class="nav__link">
                <ion-icon name="log-out-outline" class="nav__icon"></ion-icon>
                <span class="nav__name">Sair</span>
            </a>
        </nav>
    </div>

    <section class="container-fluid">
        <div class="row">
            <div class="col-md-10">
                <div class="border-bottom" class="titulo">
                    <h1>Importantes</h1>
                </div>
            </div>
            <div class="col-2">
                <div>
                    <a href="login.html">
                        <button type="button" class="btn btn-dark"><i class="fa-solid fa-right-from-bracket"></i>
                            Sair</button>
                    </a>
                </div>
            </div>
        </div>

        <div class="row">
            <div class="col-md-2 pt-2">
                <link href="https://maxcdn.bootstrapcdn.com/font-awesome/4.3.0/css/font-awesome.min.css"
                    rel="stylesheet">
                <button type="button" class="btn btn-primary" data-bs-toggle="modal" data-bs-target="#modal1">
                    Enviar Mensagem
                </button>
                <hr>
                <div>
                    <ul>
                        <li class="header"><strong>Pastas</strong></li>
                        <li><a href="mensagem.html"><i class="fa fa-envelope"></i> Caixa de Entrada</a></li>
                        <li><a href="caixadesaida.html"><i class="fa fa-envelope-o"></i> Caixa de Saída</a></li>
                        <li><a href="importantes.html"><i class="fa fa-bookmark"></i> Importantes</a></li>
                        <li><a href="Lixeira.html"><i class="fa fa-pencil-square-o"></i> Lixeira</a></li>
                    </ul>
                </div>
            </div>

            <!-- BEGIN INBOX CONTENT -->
            <div class="col-md-9">
                <div class="row">
                    <div class="col-sm-6">
                        <label style="margin-right: 8px;" class="">
                            <div class="icheckbox_square-blue" style="position: relative;"><input type="checkbox"
                                    id="check-all" class="icheck"
                                    style="position: absolute; top: -20%; left: -20%; display: block; width: 140%; height: 140%; margin: 0px; padding: 0px; border: 0px; opacity: 0; background: rgb(255, 255, 255);"><ins
                                    class="iCheck-helper"
                                    style="position: absolute; top: -20%; left: -20%; display: block; width: 140%; height: 140%; margin: 0px; padding: 0px; border: 0px; opacity: 0; background: rgb(255, 255, 255);"></ins>
                            </div>
                        </label>
                        <div class="btn-group pt-4">
                            <button type="button" class="btn btn-default dropdown-toggle" data-toggle="dropdown">
                                Filtro <span class="caret"></span>
                            </button>
                            <ul class="dropdown-menu" role="menu">
                                <li><a href="#">Mark as read</a></li>
                                <li><a href="#">Mark as unread</a></li>
                                <li><a href="#">Mark as important</a></li>
                                <li><a href="#">Delete</a></li>
                            </ul>
                        </div>
                    </div>

                    <div class="col-md-6 search-form pt-2 pb-2 ">
                        <form action="#" class="text-right">
                            <div class="input-group">
                                <form class="d-flex" role="search">
                                    <input class="form-control me-2" type="search" placeholder="Pesquisar"
                                        aria-label="Search">
                                    <button class="btn btn-outline-success" type="submit">Pesquisar</button>
                                </form>
                        </form>
                    </div>
                </div>

                <div class="padding"></div>
                <div class="text-dark mx-2">
                    <h6>Você selecionou apenas mensagens importantes.
                    </h6>
                </div>

                <div class="table-responsive ">
                    <table class="table">
                        <tbody>

                            <tr>
                                <td class="action"><input type="checkbox" /></td>
                                <td class="action"><i class="fa fa-bookmark"></i></td>
                                <td class="name"><a href="#" data-bs-toggle="modal" data-bs-target="#">Gabriel Alvez</a>
                                </td>
                                <td class="subject"><a href="#" data-bs-toggle="modal" data-bs-target="#">Boa tarde
                                        mentor, tem com o me ajudar com o vetor em c...</a></td>
                                <td class="time">15:30 PM</td>
                            </tr>

                        </tbody>
                    </table>
                </div>

                <nav>
                    <ul class="pagination">
                        <li class="page-item">
                            <a class="page-link" href="#">Voltar</a>
                        </li>
                        <li class="page-item"><a class="page-link" href="#">1</a></li>
                        <li class="page-item" aria-current="page">
                            <a class="page-link" href="#">2</a>
                        </li>
                        <li class="page-item"><a class="page-link" href="#">3</a></li>
                        <li class="page-item">
                            <a class="page-link" href="#">Proxima</a>
                        </li>
                    </ul>
                </nav>
                <!-- END INBOX CONTENT -->

            </div>
        </div>
        </div>

        <!-- Modal 1 -->
        <div class="modal fade" id="modal1" tabindex="-1" aria-labelledby="exampleModalLabel" aria-hidden="true">
            <div class="modal-dialog">
                <div class="modal-content">
                    <div class="modal-header">
                        <h1 class="modal-title fs-5" id="exampleModalLabel">Nova mensagem</h1>
                        <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
                    </div>
                    <div class="modal-body">
                        <main>
                            <div class="panel-body contacts">
                                <button type="button" class="btn btn-primary" data-bs-toggle="modal"
                                    data-bs-target="#modal3"><i class="fa-solid fa-address-book"></i>
                                    Contatos
                                </button>
                            </div>
                            <form>
                                <div class="form-row mb-3">
                                    <label for="to" class="col-2 col-sm-1 col-form-label">Para:</label>
                                    <div class="col-10 col-sm-11">
                                        <input type="email" class="form-control" id="to" placeholder="email">
                                    </div>
                                </div>
                                <div class="form-row mb-3">
                                    <label for="cc" class="col-2 col-sm-1 col-form-label">Assunto:</label>
                                    <div class="col-10 col-sm-11">
                                        <input type="email" class="form-control" id="cc" placeholder="assunto">
                                    </div>
                                </div>

                                <div class="form-row mb-3">
                                    <label for="cc" class="col-2 col-sm-1 col-form-label">CC:</label>
                                    <div class="col-10 col-sm-11">
                                        <input type="email" class="form-control" id="cc" placeholder="copias">
                                    </div>
                                </div>

                            </form>
                            <div class="row">
                                <div class="col-sm-11 ml-auto">
                                    <div class="toolbar" role="toolbar">
                                        <div class="btn-group">
                                            <button type="button" class="btn btn-light">
                                                <span class="fa fa-bold"></span>
                                            </button>
                                            <button type="button" class="btn btn-light">
                                                <span class="fa fa-italic"></span>
                                            </button>
                                            <button type="button" class="btn btn-light">
                                                <span class="fa fa-underline"></span>
                                            </button>
                                        </div>

                                        <button type="button" class="btn btn-light">
                                            <span class="fa fa-trash-o"></span>
                                        </button>
                                        <button type="button" class="btn btn-light">
                                            <span class="fa fa-paperclip"></span>
                                        </button>
                                    </div>
                                    <div class="form-group mt-4">
                                        <textarea class="form-control" id="message" name="body" rows="12"
                                            placeholder="escrever"></textarea>
                                    </div>
                                    <div class="form-group mt-4">
                                        <button type="submit" class="btn btn-danger"
                                            data-bs-dismiss="modal">Cancelar</button>
                                        <button type="submit" class="btn btn-success">Enviar</button>
                                    </div>
                                </div>
                            </div>
                        </main>
                    </div>
                    <div class="modal-footer">
                        <button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Fechar</button>
                    </div>
                </div>
            </div>



            <script>
                document.addEventListener('DOMContentLoaded', function () {
                    document.querySelector('#modal1 .btn-success').addEventListener('click', function () {
                        alert('Mensagem enviada com sucesso!');
                        $('#modal1').modal('hide');
                    });
                });
            </script>
        </div>
        <!-- Modal 1 FIM -->

        <!-- Modal 2 -->
        <div class="modal fade" id="modal2" tabindex="-1" aria-labelledby="exampleModalLabel" aria-hidden="true">
            <div class="modal-dialog">
                <div class="modal-content">
                    <div class="modal-header">
                        <h1 class="modal-title fs-5" id="exampleModalLabel">Caixa de entrada</h1>
                        <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
                    </div>
                    <div class="modal-body">
                        <main>
                            <link href="https://maxcdn.bootstrapcdn.com/font-awesome/4.3.0/css/font-awesome.min.css"
                                rel="stylesheet">
                            <div class="container">
                                <div class="row inbox">
                                    <div class="col-md-3">
                                        <div class="panel panel-default">
                                            <div class="panel-body inbox-menu">
                                                <a href="#" data-bs-toggle="modal" data-bs-target="#modal1"
                                                    class="btn btn-danger btn-block">Enviar Mensagem </a>
                                                <ul>
                                                    <li>
                                                        <a href="mensagem.html"><i class="fa fa-inbox"></i> Caixa de
                                                            Entrada <span class="label label-danger"></span></a>
                                                    </li>
                                                    <li>
                                                        <a href="#"><i class="fa fa-rocket"></i> Caixa de Saída</a>
                                                    </li>
                                                    <li>
                                                        <a href="#"><i class="fa fa-trash-o"></i> Lixo</a>
                                                    </li>
                                                    <li>
                                                        <a href="#"><i class="fa fa-bookmark"></i> Importantes<span
                                                                class="label label-info"></span></a>
                                                    </li>
                                                    <li class="title">
                                                </ul>
                                            </div>
                                        </div>
                                        <div class="panel panel-default">
                                            <div class="panel-body contacts">
                                                <button type="button" class="btn btn-primary" data-bs-toggle="modal"
                                                    data-bs-target="#modal3"><i class="fa-solid fa-address-book"></i>
                                                    Contatos
                                                </button>
                                            </div>
                                        </div>
                                    </div><!--/.col-->
                                    <div class="col-md-9">
                                        <div class="panel panel-default">
                                            <div class="panel-body message">
                                                <span class="btn-group">

                                                    <button class="btn btn-default"><span
                                                            class="fa fa-bookmark-o"></span></button>
                                                </span>
                                                <span class="btn-group">
                                                    <button class="btn btn-default"><span
                                                            class="fa fa-mail-reply"></span></button>
                                                    <button class="btn btn-default"><span
                                                            class="fa fa-mail-reply-all"></span></button>
                                                    <button class="btn btn-default"><span
                                                            class="fa fa-mail-forward"></span></button>
                                                </span>
                                                <button class="btn btn-default"><span
                                                        class="fa fa-trash-o"></span></button>

                                                <div class="message-title">Dificuldade em Switch </div>
                                                <div class="header">
                                                    <img class="avatar"
                                                        src="https://bootdey.com/img/Content/avatar/avatar1.png">
                                                    <div class="from">
                                                        <span>Clenilson Junior</span>
                                                        clenilsonjunior@holeczek.pl
                                                    </div>
                                                    <div class="date"><span class="fa fa-paper-clip"></span> Today,
                                                        <b>3:47 PM</b>
                                                    </div>
                                                    <div class="menu"></div>
                                                </div>
                                                <div class="content">
                                                    <p>
                                                        Olá, mentor! Tenho enfrentado algumas dificuldades com a
                                                        programação em C#. Sinto que preciso de ajuda para entender
                                                        melhor os conceitos de switch. Será que você pode me orientar?
                                                    </p>
                                                    <blockquote>
                                                        <!---->
                                                    </blockquote>
                                                </div>
                                                <div class="attachments">
                                                    <ul>
                                                        <li>
                                                            <span class="label label-danger">zip</span>
                                                            <b>bootstrap.zip</b> <i>(2,5MB)</i>
                                                            <span class="quickMenu">
                                                                <a href="#" class="fa fa-search"><i></i></a>
                                                                <a href="#" class="fa fa-share"><i></i></a>
                                                                <a href="#" class="fa fa-cloud-download"><i></i></a>
                                                            </span>
                                                        </li>
                                                        <li>
                                                            <span class="label label-info">txt</span> <b>readme.txt</b>
                                                            <i>(7KB)</i>
                                                            <span class="quickMenu">
                                                                <a href="#" class="fa fa-search"><i></i></a>
                                                                <a href="#" class="fa fa-share"><i></i></a>
                                                                <a href="#" class="fa fa-cloud-download"><i></i></a>
                                                            </span>
                                                        </li>
                                                        <li>
                                                            <span class="label label-success">xls</span>
                                                            <b>spreadsheet.xls</b> <i>(984KB)</i>
                                                            <span class="quickMenu">
                                                                <a href="#" class="fa fa-search"><i></i></a>
                                                                <a href="#" class="fa fa-share"><i></i></a>
                                                                <a href="#" class="fa fa-cloud-download"><i></i></a>
                                                            </span>
                                                        </li>
                                                    </ul>
                                                </div>
                                                <form method="post" action="">
                                                    <div class="form-group">
                                                        <textarea class="form-control" id="message" name="body"
                                                            rows="12" placeholder="escreva"></textarea>
                                                    </div>
                                                    <div class="form-group pt-2">
                                                        <button tabindex="3" type="submit"
                                                            class="btn btn-success">Responder</button>
                                                    </div>
                                                </form>
                                            </div>
                                        </div>
                                    </div><!--/.col-->
                                </div>
                            </div>
                        </main>
                    </div>
                    <div class="modal-footer">
                        <button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Fechar</button>
                    </div>
                </div>
            </div>
        </div>
        <!-- Modal 2 FIM -->

        <!-- Modal 3  -->
        <div class="modal fade" id="modal3" tabindex="-1" aria-labelledby="exampleModalLabel" aria-hidden="true">
            <div class="modal-dialog">
                <div class="modal-content">
                    <div class="modal-header">
                        <h1 class="modal-title fs-5" id="exampleModalLabel">Contatos</h1>
                        <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
                    </div>
                    <div class="modal-body">
                        <div class="container">
                            <div class="row align-items-center">
                                <div class="row">
                                    <div class="col-xl-3 col-sm-6">
                                        <div class="card">
                                            <div class="card-body">
                                                <div class="d-flex align-items-center">
                                                    <div><img src="https://bootdey.com/img/Content/avatar/avatar1.png"
                                                            alt="" class="avatar-md rounded-circle img-thumbnail" />
                                                    </div>
                                                    <div class="flex-1 ms-3">
                                                        <h5 class="font-size-16 mb-1"><a href="#"
                                                                class="text-dark">Phyllis Gatlin</a></h5>
                                                        <span class="badge badge-soft-success mb-0">Full Stack
                                                            Developer</span>
                                                    </div>
                                                </div>
                                                <div class="mt-3 pt-1">
                                                    <p class="text-muted mb-0"><i
                                                            class="mdi mdi-phone font-size-15 align-middle pe-2 text-primary"></i>
                                                        070 2860 5375</p>
                                                    <p class="text-muted mb-0 mt-2"><i
                                                            class="mdi mdi-email font-size-15 align-middle pe-2 text-primary"></i>
                                                        PhyllisGatlin@spy.com</p>
                                                    <p class="text-muted mb-0 mt-2"><i
                                                            class="mdi mdi-google-maps font-size-15 align-middle pe-2 text-primary"></i>
                                                        52 Ilchester MYBSTER 9WX</p>
                                                </div>
                                                <div class="d-flex gap-2 pt-4">
                                                    <button type="button" class="btn btn-primary btn-sm w-50"><i
                                                            class="bx bx-message-square-dots me-1"></i>
                                                        Selecionar</button>
                                                </div>
                                            </div>
                                        </div>
                                    </div>
                                    <div class="col-xl-3 col-sm-6">
                                        <div class="card">
                                            <div class="card-body">
                                                <div class="d-flex align-items-center">
                                                    <div><img src="https://bootdey.com/img/Content/avatar/avatar2.png"
                                                            alt="" class="avatar-md rounded-circle img-thumbnail" />
                                                    </div>
                                                    <div class="flex-1 ms-3">
                                                        <h5 class="font-size-16 mb-1"><a href="#"
                                                                class="text-dark">James Nix</a></h5>
                                                        <span class="badge badge-soft-success mb-0">Full Stack
                                                            Developer</span>
                                                    </div>
                                                </div>
                                                <div class="mt-3 pt-1">
                                                    <p class="text-muted mb-0"><i
                                                            class="mdi mdi-phone font-size-15 align-middle pe-2 text-primary"></i>
                                                        046 5685 6969</p>
                                                    <p class="text-muted mb-0 mt-2"><i
                                                            class="mdi mdi-email font-size-15 align-middle pe-2 text-primary"></i>
                                                        JamesNix@spy.com</p>
                                                    <p class="text-muted mb-0 mt-2"><i
                                                            class="mdi mdi-google-maps font-size-15 align-middle pe-2 text-primary"></i>
                                                        5 Boar Lane SELLING 2LG</p>
                                                </div>
                                                <div class="d-flex gap-2 pt-4">
                                                    <button type="button" class="btn btn-primary btn-sm w-50"><i
                                                            class="bx bx-message-square-dots me-1"></i>
                                                        Selecionar</button>
                                                </div>
                                            </div>
                                        </div>
                                    </div>
                                    <div class="col-xl-3 col-sm-6">
                                        <div class="card">
                                            <div class="card-body">
                                                <div class="d-flex align-items-center">
                                                    <div><img src="https://bootdey.com/img/Content/avatar/avatar3.png"
                                                            alt="" class="avatar-md rounded-circle img-thumbnail" />
                                                    </div>
                                                    <div class="flex-1 ms-3">
                                                        <h5 class="font-size-16 mb-1"><a href="#"
                                                                class="text-dark">Darlene Smith</a></h5>
                                                        <span class="badge badge-soft-danger mb-0">UI/UX Designer</span>
                                                    </div>
                                                </div>
                                                <div class="mt-3 pt-1">
                                                    <p class="text-muted mb-0"><i
                                                            class="mdi mdi-phone font-size-15 align-middle pe-2 text-primary"></i>
                                                        012 6587 1236</p>
                                                    <p class="text-muted mb-0 mt-2"><i
                                                            class="mdi mdi-email font-size-15 align-middle pe-2 text-primary"></i>
                                                        DarleneSmith@spy.com</p>
                                                    <p class="text-muted mb-0 mt-2"><i
                                                            class="mdi mdi-google-maps font-size-15 align-middle pe-2 text-primary"></i>
                                                        57 Guildry Street GAMRIE</p>
                                                </div>
                                                <div class="d-flex gap-2 pt-4">
                                                    <button type="button" class="btn btn-primary btn-sm w-50"><i
                                                            class="bx bx-message-square-dots me-1"></i>
                                                        Selecionar</button>
                                                </div>
                                            </div>
                                        </div>
                                    </div>
                                    <div class="col-xl-3 col-sm-6">
                                        <div class="card">
                                            <div class="card-body">
                                                <div class="d-flex align-items-center">
                                                    <div class="avatar-md">
                                                        <div
                                                            class="avatar-title bg-soft-primary text-primary display-6 m-0 rounded-circle">
                                                            <i class="bx bxs-user-circle"></i>
                                                        </div>
                                                    </div>
                                                    <div class="flex-1 ms-3">
                                                        <h5 class="font-size-16 mb-1"><a href="#"
                                                                class="text-dark">William Swift</a></h5>
                                                        <span class="badge badge-soft-warning mb-0">Backend
                                                            Developer</span>
                                                    </div>
                                                </div>
                                                <div class="mt-3 pt-1">
                                                    <p class="text-muted mb-0"><i
                                                            class="mdi mdi-phone font-size-15 align-middle pe-2 text-primary"></i>
                                                        012 6587 1236</p>
                                                    <p class="text-muted mb-0 mt-2"><i
                                                            class="mdi mdi-email font-size-15 align-middle pe-2 text-primary"></i>
                                                        WilliamSwift@spy.com</p>
                                                    <p class="text-muted mb-0 mt-2"><i
                                                            class="mdi mdi-google-maps font-size-15 align-middle pe-2 text-primary"></i>
                                                        80 South Street MONKW 7BR</p>
                                                </div>
                                                <div class="d-flex gap-2 pt-4">
                                                    <button type="button" class="btn btn-primary btn-sm w-50"><i
                                                            class="bx bx-message-square-dots me-1"></i>
                                                        Selecionar</button>
                                                </div>
                                            </div>
                                        </div>
                                    </div>
                                    <div class="col-xl-3 col-sm-6">
                                        <div class="card">
                                            <div class="card-body">
                                                <div class="d-flex align-items-center">
                                                    <div class="avatar-md">
                                                        <div
                                                            class="avatar-title bg-soft-primary text-primary display-6 m-0 rounded-circle">
                                                            <i class="bx bxs-user-circle"></i>
                                                        </div>
                                                    </div>
                                                    <div class="flex-1 ms-3">
                                                        <h5 class="font-size-16 mb-1"><a href="#"
                                                                class="text-dark">Kevin West</a></h5>
                                                        <span class="badge badge-soft-success mb-0">Full Stack
                                                            Developer</span>
                                                    </div>
                                                </div>
                                                <div class="mt-3 pt-1">
                                                    <p class="text-muted mb-0"><i
                                                            class="mdi mdi-phone font-size-15 align-middle pe-2 text-primary"></i>
                                                        052 6524 9896</p>
                                                    <p class="text-muted mb-0 mt-2"><i
                                                            class="mdi mdi-email font-size-15 align-middle pe-2 text-primary"></i>
                                                        KevinWest@spy.com</p>
                                                    <p class="text-muted mb-0 mt-2"><i
                                                            class="mdi mdi-google-maps font-size-15 align-middle pe-2 text-primary"></i>
                                                        88 Tadcaster PINCHBECK 6UB</p>
                                                </div>
                                                <div class="d-flex gap-2 pt-4">
                                                    <button type="button" class="btn btn-primary btn-sm w-50"><i
                                                            class="bx bx-message-square-dots me-1"></i>
                                                        Selecionar</button>
                                                </div>
                                            </div>
                                        </div>
                                    </div>
                                    <div class="col-xl-3 col-sm-6">
                                        <div class="card">
                                            <div class="card-body">
                                                <div class="d-flex align-items-center">
                                                    <div><img src="https://bootdey.com/img/Content/avatar/avatar4.png"
                                                            alt="" class="avatar-md rounded-circle img-thumbnail" />
                                                    </div>
                                                    <div class="flex-1 ms-3">
                                                        <h5 class="font-size-16 mb-1"><a href="#"
                                                                class="text-dark">Tommy Hayes</a></h5>
                                                        <span class="badge badge-soft-warning mb-0">Backend
                                                            Developer</span>
                                                    </div>
                                                </div>
                                                <div class="mt-3 pt-1">
                                                    <p class="text-muted mb-0"><i
                                                            class="mdi mdi-phone font-size-15 align-middle pe-2 text-primary"></i>
                                                        065 2563 6587</p>
                                                    <p class="text-muted mb-0 mt-2"><i
                                                            class="mdi mdi-email font-size-15 align-middle pe-2 text-primary"></i>
                                                        TommyHayes@spy.com</p>
                                                    <p class="text-muted mb-0 mt-2"><i
                                                            class="mdi mdi-google-maps font-size-15 align-middle pe-2 text-primary"></i>
                                                        5 Boar Lane SELLING 2LG</p>
                                                </div>
                                                <div class="d-flex gap-2 pt-4">
                                                    <button type="button" class="btn btn-primary btn-sm w-50"><i
                                                            class="bx bx-message-square-dots me-1"></i>
                                                        Selecionar</button>
                                                </div>
                                            </div>
                                        </div>
                                    </div>
                                    <div class="col-xl-3 col-sm-6">
                                        <div class="card">
                                            <div class="card-body">
                                                <div class="d-flex align-items-center">
                                                    <div><img src="https://bootdey.com/img/Content/avatar/avatar5.png"
                                                            alt="" class="avatar-md rounded-circle img-thumbnail" />
                                                    </div>
                                                    <div class="flex-1 ms-3">
                                                        <h5 class="font-size-16 mb-1"><a href="#"
                                                                class="text-dark">Diana Owens</a></h5>
                                                        <span class="badge badge-soft-danger mb-0">UI/UX Designer</span>
                                                    </div>
                                                </div>
                                                <div class="mt-3 pt-1">
                                                    <p class="text-muted mb-0"><i
                                                            class="mdi mdi-phone font-size-15 align-middle pe-2 text-primary"></i>
                                                        087 6321 3235</p>
                                                    <p class="text-muted mb-0 mt-2"><i
                                                            class="mdi mdi-email font-size-15 align-middle pe-2 text-primary"></i>
                                                        DianaOwens@spy.com</p>
                                                    <p class="text-muted mb-0 mt-2"><i
                                                            class="mdi mdi-google-maps font-size-15 align-middle pe-2 text-primary"></i>
                                                        52 Ilchester MYBSTER 9WX</p>
                                                </div>
                                                <div class="d-flex gap-2 pt-4">
                                                    <button type="button" class="btn btn-primary btn-sm w-50"><i
                                                            class="bx bx-message-square-dots me-1"></i>
                                                        Selecionar</button>
                                                </div>
                                            </div>
                                        </div>
                                    </div>
                                    <div class="col-xl-3 col-sm-6">
                                        <div class="card">
                                            <div class="card-body">
                                                <div class="d-flex align-items-center">
                                                    <div><img src="https://bootdey.com/img/Content/avatar/avatar6.png"
                                                            alt="" class="avatar-md rounded-circle img-thumbnail" />
                                                    </div>
                                                    <div class="flex-1 ms-3">
                                                        <h5 class="font-size-16 mb-1"><a href="#" class="text-dark">Paul
                                                                Sanchez</a></h5>
                                                        <span class="badge badge-soft-success mb-0">Full Stack
                                                            Developer</span>
                                                    </div>
                                                </div>
                                                <div class="mt-3 pt-1">
                                                    <p class="text-muted mb-0"><i
                                                            class="mdi mdi-phone font-size-15 align-middle pe-2 text-primary"></i>
                                                        021 0125 5689</p>
                                                    <p class="text-muted mb-0 mt-2"><i
                                                            class="mdi mdi-email font-size-15 align-middle pe-2 text-primary"></i>
                                                        DianaOwens@spy.com</p>
                                                    <p class="text-muted mb-0 mt-2"><i
                                                            class="mdi mdi-google-maps font-size-15 align-middle pe-2 text-primary"></i>
                                                        80 South Street MONKW 7BR</p>
                                                </div>
                                                <div class="d-flex gap-2 pt-4">
                                                    <button type="button" class="btn btn-primary btn-sm w-50"><i
                                                            class="bx bx-message-square-dots me-1"></i>
                                                        Selecionar</button>
                                                </div>
                                            </div>
                                        </div>
                                    </div>
                                </div>
                                <div class="row g-0 align-items-center pb-4">
                                    <div class="col-sm-11">
                                        <div class="float-sm-end">
                                            <nav aria-label="...">
                                                <ul class="pagination pagination-sm">
                                                    <li class="page-item active" aria-current="page">
                                                        <span class="page-link">1</span>
                                                    </li>
                                                    <li class="page-item"><a class="page-link" href="#">2</a></li>
                                                    <li class="page-item"><a class="page-link" href="#">3</a></li>
                                                </ul>
                                            </nav>
                                        </div>
                                    </div>
                                </div>
                            </div>
                            <div class="modal-footer">
                                <button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Fechar</button>
                            </div>
                        </div>
                    </div>
                </div>

    </section>



    <!-- ===== IONICONS ===== -->
    <script src="https://unpkg.com/ionicons@5.1.2/dist/ionicons.js"></script>

    <!-- ===== MAIN JS ===== -->
    <script src="assets/js/main.js"></script>

    <!-- ===== BOOTSTRAP ===== -->
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.bundle.min.js"
        integrity="sha384-C6RzsynM9kWDrMNeT87bh95OGNyZPhcTNXj1NW7RuBCsyN/o0jlpcV8Qyq46cDfL"
        crossorigin="anonymous"></script>
</body>

</html>

------------------ Lixeira.html-------------------
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <!-- ===== BOOTSTRAP ===== -->
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/css/bootstrap.min.css" rel="stylesheet"
        integrity="sha384-T3c6CoIi6uLrA9TneNEoa7RxnatzjcDSCmG1MXxSR1GAsXEV/Dwwykc2MPK8M2HN" crossorigin="anonymous">
    <!-- ===== CSS ===== -->
    <link rel="stylesheet" href="assets/css/styles.css">
    <!-- ===== ICON ===== -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.2/css/all.min.css"
        integrity="sha512-z3gLpd7yknf1YoNbCzqRKc4qyor8gaKU1qmn+CShxbuBusANI9QpRohGBreCFkKxLhei6S9CQXFEbbKuqLg0DA=="
        crossorigin="anonymous" referrerpolicy="no-referrer" />

    <title>PUC Minas - Programa de Monitoria</title>
</head>

<body id="body-pd">
    <div class="l-navbar" id="navbar">
        <nav class="nav">
            <div>
                <div class="nav__brand">
                    <ion-icon name="menu-outline" class="nav__toggle" id="nav-toggle"></ion-icon>
                    <a href="Lixeira.html" class="nav__logo"><img id="logo" src="assets/img/logo.png"
                            width="15%"></a>
                </div>

                <div class="nav__list">
                    <a href="painel_aluno.html" class="nav__link active">
                        <ion-icon name="home-outline" class="nav__icon"></ion-icon>
                        <span class="nav__name">Painel de Controle</span>
                    </a>

                    <a href="mensagem.html" class="nav__link">
                        <ion-icon name="chatbubbles-outline" class="nav__icon"></ion-icon>
                        <span class="nav__name">Mensagem</span>
                    </a>

                    <a href="agenda.html" class="nav__link">
                        <ion-icon name="calendar-outline" class="nav__icon"></ion-icon>
                        <span class="nav__name">Calendario</span>
                    </a>

                    <a href="https://teams.microsoft.com/dl/launcher/launcher.html?url=teams&type=meetup-join&enableMobilePage=true&suppressPrompt=true&tenantId=14cbd5a7-ec94-46ba-b314-cc0fc972a161"
                        class="nav__link">
                        <ion-icon name="tv" class="nav__icon"></ion-icon>
                        <span class="nav__name">Teams</span>
                    </a>


                    <a href="ajuda.html" class="nav__link">
                        <ion-icon name="help-outline" class="nav__icon"></ion-icon>
                        <span class="nav__name">Ajuda</span>
                    </a>

                    <a href="config.html" class="nav__link">
                        <ion-icon name="settings-outline" class="nav__icon"></ion-icon>
                        <span class="nav__name">Configurações</span>
                    </a>
                </div>
            </div>



            <div>
                <img id="foto" src="assets/img/foto.png" width="12%">
            </div>

            <a href="login.html" class="nav__link">
                <ion-icon name="log-out-outline" class="nav__icon"></ion-icon>
                <span class="nav__name">Sair</span>
            </a>
        </nav>
    </div>

    <section class="container-fluid">
        <div class="row">
            <div class="col-md-10">
                <div class="border-bottom" class="titulo">
                    <h1>Lixeira</h1>
                </div>
            </div>
            <div class="col-2">
                <div>
                    <a href="login.html">
                    <button type="button" class="btn btn-dark"><i class="fa-solid fa-right-from-bracket"></i> Sair</button>
                </a>
                </div>
            </div>
        </div>

        <div class="row">
            <div class="col-md-2 pt-2">
                <link href="https://maxcdn.bootstrapcdn.com/font-awesome/4.3.0/css/font-awesome.min.css"
                    rel="stylesheet">
                <button id="btnEsvaziarLixeira" type="button" class="btn btn-primary" data-bs-toggle="modal" data-bs-target="#modal1"><i class="fa-solid fa-trash"></i>
                    Esvaziar Lixeira
                </button>
                <hr>
                <div>
                    <ul>
                        <li class="header"><strong>Pastas</strong></li>
                        <li><a href="mensagem.html"><i class="fa fa-envelope"></i> Caixa de Entrada</a></li>
                        <li><a href="caixadesaida.html"><i class="fa fa-envelope-o"></i> Caixa de Saída</a></li>
                        <li><a href="importantes.html"><i class="fa fa-bookmark"></i> Importantes</a></li>
                        <li><a href="Lixeira.html"><i class="fa fa-pencil-square-o"></i> Lixeira</a></li>
                    </ul>
                </div>
            </div>

            <script>
                document.addEventListener('DOMContentLoaded', function () {
                    document.getElementById('btnEsvaziarLixeira').addEventListener('click', function () {
                        var confirmacao = confirm('Tem certeza de que deseja esvaziar a lixeira?');
            
                        if (confirmacao) {
                            alert('Lixeira esvaziada com sucesso!');
                        }
                    });
                });
            </script>

            <!-- BEGIN INBOX CONTENT -->
            <div class="col-md-9">
                <div class="row">
                    <div class="col-sm-6">
                        <label style="margin-right: 8px;" class="">
                            <div class="icheckbox_square-blue" style="position: relative;"><input type="checkbox"
                                    id="check-all" class="icheck"
                                    style="position: absolute; top: -20%; left: -20%; display: block; width: 140%; height: 140%; margin: 0px; padding: 0px; border: 0px; opacity: 0; background: rgb(255, 255, 255);"><ins
                                    class="iCheck-helper"
                                    style="position: absolute; top: -20%; left: -20%; display: block; width: 140%; height: 140%; margin: 0px; padding: 0px; border: 0px; opacity: 0; background: rgb(255, 255, 255);"></ins>
                            </div>
                        </label>
                        <div class="btn-group pt-4">
                            <button type="button" class="btn btn-default dropdown-toggle" data-toggle="dropdown">
                                Filtro <span class="caret"></span>
                            </button>
                            <ul class="dropdown-menu" role="menu">
                                <li><a href="#">Mark as read</a></li>
                                <li><a href="#">Mark as unread</a></li>
                                <li><a href="#">Mark as important</a></li>
                                <li><a href="#">Delete</a></li>
                            </ul>
                        </div>
                    </div>

                    <div class="col-md-6 search-form pt-2 pb-2 ">
                        <form action="#" class="text-right">
                            <div class="input-group">
                                <form class="d-flex" role="search">
                                    <input class="form-control me-2" type="search" placeholder="Pesquisar"
                                        aria-label="Search">
                                    <button class="btn btn-outline-success" type="submit">Pesquisar</button>
                                </form>
                        </form>
                    </div>
                </div>

                <div class="padding"></div>
                <div class="text-danger mx-2">
                    <h6>Itens excluídos, esvazie a lixeira para remover para sempre.
                    </h6>
                </div>

                <div class="table-responsive ">
                    <table class="table">
                        <tbody>
                            <tr>
                                <td class="action"><input type="checkbox" /></td>
                                <td class="action"><i class="fa fa-bookmark-o"></i></td>
                                <td class="name"><a href="#" data-bs-toggle="modal" data-bs-target="#modal2"> Paulo
                                        Silva</a></td>
                                <td class="subject"><a href="#" data-bs-toggle="modal" data-bs-target="#modal2"> Olá
                                        mentor! Poderia me ajudar com DIW? Não consegui resol... </a></td>
                                <td class="time">01:47 PM</td>
                            </tr>

                        </tbody>
                    </table>
                </div>


                <nav>
                    <ul class="pagination">
                        <li class="page-item">
                            <a class="page-link" href="#">Voltar</a>
                        </li>
                        <li class="page-item"><a class="page-link" href="#">1</a></li>
                        <li class="page-item" aria-current="page">
                            <a class="page-link" href="#">2</a>
                        </li>
                        <li class="page-item"><a class="page-link" href="#">3</a></li>
                        <li class="page-item">
                            <a class="page-link" href="#">Proxima</a>
                        </li>
                    </ul>
                </nav>
                <!-- END INBOX CONTENT -->

            </div>
        </div>
        </div>

        <!-- Modal 1 -->


        <!-- Modal 1 FIM -->

        <!-- Modal 2 -->
        <div class="modal fade" id="modal2" tabindex="-1" aria-labelledby="exampleModalLabel" aria-hidden="true">
            <div class="modal-dialog">
                <div class="modal-content">
                    <div class="modal-header">
                        <h1 class="modal-title fs-5" id="exampleModalLabel">Caixa de entrada</h1>
                        <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
                    </div>
                    <div class="modal-body">
                        <main>
                            <link href="https://maxcdn.bootstrapcdn.com/font-awesome/4.3.0/css/font-awesome.min.css"
                                rel="stylesheet">
                            <div class="container">
                                <div class="row inbox">
                                    <div class="col-md-3">
                                        <div class="panel panel-default">
                                            <div class="panel-body inbox-menu">
                                                <a href="#" data-bs-toggle="modal" data-bs-target="#modal1"
                                                    class="btn btn-danger btn-block">Enviar Mensagem </a>
                                                <ul>
                                                    <li>
                                                        <a href="mensagem.html"><i class="fa fa-inbox"></i> Caixa de
                                                            Entrada <span class="label label-danger"></span></a>
                                                    </li>
                                                    <li>
                                                        <a href="#"><i class="fa fa-rocket"></i> Caixa de Saída</a>
                                                    </li>
                                                    <li>
                                                        <a href="#"><i class="fa fa-trash-o"></i> Lixo</a>
                                                    </li>
                                                    <li>
                                                        <a href="#"><i class="fa fa-bookmark"></i> Importantes<span
                                                                class="label label-info"></span></a>
                                                    </li>
                                                    <li class="title">
                                                </ul>
                                            </div>
                                        </div>
                                        <div class="panel panel-default">
                                            <div class="panel-body contacts">
                                                <button type="button" class="btn btn-primary" data-bs-toggle="modal"
                                                    data-bs-target="#modal3"><i class="fa-solid fa-address-book"></i>
                                                    Contatos
                                                </button>
                                            </div>
                                            </div>
                                        </div>
                                    </div><!--/.col-->
                                    <div class="col-md-9">
                                        <div class="panel panel-default">
                                            <div class="panel-body message">
                                                <span class="btn-group">

                                                    <button class="btn btn-default"><span
                                                            class="fa fa-bookmark-o"></span></button>
                                                </span>
                                                <span class="btn-group">
                                                    <button class="btn btn-default"><span
                                                            class="fa fa-mail-reply"></span></button>
                                                    <button class="btn btn-default"><span
                                                            class="fa fa-mail-reply-all"></span></button>
                                                    <button class="btn btn-default"><span
                                                            class="fa fa-mail-forward"></span></button>
                                                </span>
                                                <button class="btn btn-default"><span
                                                        class="fa fa-trash-o"></span></button>

                                                <div class="message-title">Dificuldade em DIW</div>
                                                <div class="header">
                                                    <img class="avatar"
                                                        src="https://bootdey.com/img/Content/avatar/avatar2.png">
                                                    <div class="from text-dark">
                                                        <span>Paulo Silva</span>
                                                        PauloSilva@holeczek.pl
                                                    </div>
                                                    <div class="date"><span class="fa fa-paper-clip"></span> Today,
                                                        <b>01:47 PM</b>
                                                    </div>
                                                    <div class="menu"></div>
                                                </div>
                                                <div class="content">
                                                    <p>
                                                        Olá mentor! Poderia me ajudar com DIW? Não consegui resolver a
                                                        atividade que ele passou de 2 pontos sobre Javascript, Pode me
                                                        socorrer?

                                                    </p>
                                                    <blockquote>
                                                        <!---->
                                                    </blockquote>
                                                    <div class="header">
                                                        <img class="avatar"
                                                            src="https://bootdey.com/img/Content/avatar/avatar2.png">
                                                        <div class="from text-dark">
                                                            <span>Paulo Silva</span>
                                                            PauloSilva@holeczek.pl
                                                        </div>
                                                        <div class="date"><span class="fa fa-paper-clip"></span> Today,
                                                            <b>05:03 PM</b>
                                                        </div>
                                                        <div class="menu"></div>
                                                    </div>

                                                    <div class="content">
                                                        <p>
                                                            Não precisarei mais Mentor! Obrigado desde já, vi umas aulas
                                                            no youtube que
                                                            respondeu claramente minha dúvida.

                                                        </p>


                                                    </div>



                                                    <div class="attachments">
                                                        <ul>
                                                            <li>
                                                                <span class="label label-danger">zip</span>
                                                                <b>bootstrap.zip</b> <i>(2,5MB)</i>
                                                                <span class="quickMenu">
                                                                    <a href="#" class="fa fa-search"><i></i></a>
                                                                    <a href="#" class="fa fa-share"><i></i></a>
                                                                    <a href="#" class="fa fa-cloud-download"><i></i></a>
                                                                </span>
                                                            </li>
                                                            <li>
                                                                <span class="label label-info">txt</span>
                                                                <b>readme.txt</b>
                                                                <i>(7KB)</i>
                                                                <span class="quickMenu">
                                                                    <a href="#" class="fa fa-search"><i></i></a>
                                                                    <a href="#" class="fa fa-share"><i></i></a>
                                                                    <a href="#" class="fa fa-cloud-download"><i></i></a>
                                                                </span>
                                                            </li>
                                                            <li>
                                                                <span class="label label-success">xls</span>
                                                                <b>spreadsheet.xls</b> <i>(984KB)</i>
                                                                <span class="quickMenu">
                                                                    <a href="#" class="fa fa-search"><i></i></a>
                                                                    <a href="#" class="fa fa-share"><i></i></a>
                                                                    <a href="#" class="fa fa-cloud-download"><i></i></a>
                                                                </span>
                                                            </li>
                                                        </ul>
                                                    </div>
                                                    <form method="post" action="">
                                                        <div class="form-group">
                                                            <textarea class="form-control" id="message" name="body"
                                                                rows="12" placeholder="escreva"></textarea>
                                                        </div>
                                                        <div class="form-group pt-2">
                                                            <button tabindex="3" type="submit"
                                                                class="btn btn-success">Responder</button>
                                                        </div>
                                                    </form>
                                                </div>
                                            </div>
                                        </div><!--/.col-->
                                    </div>
                                </div>
                        </main>
                    </div>
                    <div class="modal-footer">
                        <button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Fechar</button>
                    </div>
                </div>
            </div>
        </div>
        <!-- Modal 2 FIM -->

        <!-- Modal 3  -->
        <div class="modal fade" id="modal3" tabindex="-1" aria-labelledby="exampleModalLabel" aria-hidden="true">
            <div class="modal-dialog">
                <div class="modal-content">
                    <div class="modal-header">
                        <h1 class="modal-title fs-5" id="exampleModalLabel">Contatos</h1>
                        <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
                    </div>
                    <div class="modal-body">
                        <div class="container">
                            <div class="row align-items-center">
                                <div class="row">
                                    <div class="col-xl-3 col-sm-6">
                                        <div class="card">
                                            <div class="card-body">
                                                <div class="d-flex align-items-center">
                                                    <div><img src="https://bootdey.com/img/Content/avatar/avatar1.png"
                                                            alt="" class="avatar-md rounded-circle img-thumbnail" />
                                                    </div>
                                                    <div class="flex-1 ms-3">
                                                        <h5 class="font-size-16 mb-1"><a href="#"
                                                                class="text-dark">Phyllis Gatlin</a></h5>
                                                        <span class="badge badge-soft-success mb-0">Full Stack
                                                            Developer</span>
                                                    </div>
                                                </div>
                                                <div class="mt-3 pt-1">
                                                    <p class="text-muted mb-0"><i
                                                            class="mdi mdi-phone font-size-15 align-middle pe-2 text-primary"></i>
                                                        070 2860 5375</p>
                                                    <p class="text-muted mb-0 mt-2"><i
                                                            class="mdi mdi-email font-size-15 align-middle pe-2 text-primary"></i>
                                                        PhyllisGatlin@spy.com</p>
                                                    <p class="text-muted mb-0 mt-2"><i
                                                            class="mdi mdi-google-maps font-size-15 align-middle pe-2 text-primary"></i>
                                                        52 Ilchester MYBSTER 9WX</p>
                                                </div>
                                                <div class="d-flex gap-2 pt-4">
                                                    <button type="button" class="btn btn-primary btn-sm w-50"><i
                                                            class="bx bx-message-square-dots me-1"></i>
                                                        Selecionar</button>
                                                </div>
                                            </div>
                                        </div>
                                    </div>
                                    <div class="col-xl-3 col-sm-6">
                                        <div class="card">
                                            <div class="card-body">
                                                <div class="d-flex align-items-center">
                                                    <div><img src="https://bootdey.com/img/Content/avatar/avatar2.png"
                                                            alt="" class="avatar-md rounded-circle img-thumbnail" />
                                                    </div>
                                                    <div class="flex-1 ms-3">
                                                        <h5 class="font-size-16 mb-1"><a href="#"
                                                                class="text-dark">James Nix</a></h5>
                                                        <span class="badge badge-soft-success mb-0">Full Stack
                                                            Developer</span>
                                                    </div>
                                                </div>
                                                <div class="mt-3 pt-1">
                                                    <p class="text-muted mb-0"><i
                                                            class="mdi mdi-phone font-size-15 align-middle pe-2 text-primary"></i>
                                                        046 5685 6969</p>
                                                    <p class="text-muted mb-0 mt-2"><i
                                                            class="mdi mdi-email font-size-15 align-middle pe-2 text-primary"></i>
                                                        JamesNix@spy.com</p>
                                                    <p class="text-muted mb-0 mt-2"><i
                                                            class="mdi mdi-google-maps font-size-15 align-middle pe-2 text-primary"></i>
                                                        5 Boar Lane SELLING 2LG</p>
                                                </div>
                                                <div class="d-flex gap-2 pt-4">
                                                    <button type="button" class="btn btn-primary btn-sm w-50"><i
                                                            class="bx bx-message-square-dots me-1"></i>
                                                        Selecionar</button>
                                                </div>
                                            </div>
                                        </div>
                                    </div>
                                    <div class="col-xl-3 col-sm-6">
                                        <div class="card">
                                            <div class="card-body">
                                                <div class="d-flex align-items-center">
                                                    <div><img src="https://bootdey.com/img/Content/avatar/avatar3.png"
                                                            alt="" class="avatar-md rounded-circle img-thumbnail" />
                                                    </div>
                                                    <div class="flex-1 ms-3">
                                                        <h5 class="font-size-16 mb-1"><a href="#"
                                                                class="text-dark">Darlene Smith</a></h5>
                                                        <span class="badge badge-soft-danger mb-0">UI/UX Designer</span>
                                                    </div>
                                                </div>
                                                <div class="mt-3 pt-1">
                                                    <p class="text-muted mb-0"><i
                                                            class="mdi mdi-phone font-size-15 align-middle pe-2 text-primary"></i>
                                                        012 6587 1236</p>
                                                    <p class="text-muted mb-0 mt-2"><i
                                                            class="mdi mdi-email font-size-15 align-middle pe-2 text-primary"></i>
                                                        DarleneSmith@spy.com</p>
                                                    <p class="text-muted mb-0 mt-2"><i
                                                            class="mdi mdi-google-maps font-size-15 align-middle pe-2 text-primary"></i>
                                                        57 Guildry Street GAMRIE</p>
                                                </div>
                                                <div class="d-flex gap-2 pt-4">
                                                    <button type="button" class="btn btn-primary btn-sm w-50"><i
                                                            class="bx bx-message-square-dots me-1"></i>
                                                        Selecionar</button>
                                                </div>
                                            </div>
                                        </div>
                                    </div>
                                    <div class="col-xl-3 col-sm-6">
                                        <div class="card">
                                            <div class="card-body">
                                                <div class="d-flex align-items-center">
                                                    <div class="avatar-md">
                                                        <div
                                                            class="avatar-title bg-soft-primary text-primary display-6 m-0 rounded-circle">
                                                            <i class="bx bxs-user-circle"></i>
                                                        </div>
                                                    </div>
                                                    <div class="flex-1 ms-3">
                                                        <h5 class="font-size-16 mb-1"><a href="#"
                                                                class="text-dark">William Swift</a></h5>
                                                        <span class="badge badge-soft-warning mb-0">Backend
                                                            Developer</span>
                                                    </div>
                                                </div>
                                                <div class="mt-3 pt-1">
                                                    <p class="text-muted mb-0"><i
                                                            class="mdi mdi-phone font-size-15 align-middle pe-2 text-primary"></i>
                                                        012 6587 1236</p>
                                                    <p class="text-muted mb-0 mt-2"><i
                                                            class="mdi mdi-email font-size-15 align-middle pe-2 text-primary"></i>
                                                        WilliamSwift@spy.com</p>
                                                    <p class="text-muted mb-0 mt-2"><i
                                                            class="mdi mdi-google-maps font-size-15 align-middle pe-2 text-primary"></i>
                                                        80 South Street MONKW 7BR</p>
                                                </div>
                                                <div class="d-flex gap-2 pt-4">
                                                    <button type="button" class="btn btn-primary btn-sm w-50"><i
                                                            class="bx bx-message-square-dots me-1"></i>
                                                        Selecionar</button>
                                                </div>
                                            </div>
                                        </div>
                                    </div>
                                    <div class="col-xl-3 col-sm-6">
                                        <div class="card">
                                            <div class="card-body">
                                                <div class="d-flex align-items-center">
                                                    <div class="avatar-md">
                                                        <div
                                                            class="avatar-title bg-soft-primary text-primary display-6 m-0 rounded-circle">
                                                            <i class="bx bxs-user-circle"></i>
                                                        </div>
                                                    </div>
                                                    <div class="flex-1 ms-3">
                                                        <h5 class="font-size-16 mb-1"><a href="#"
                                                                class="text-dark">Kevin West</a></h5>
                                                        <span class="badge badge-soft-success mb-0">Full Stack
                                                            Developer</span>
                                                    </div>
                                                </div>
                                                <div class="mt-3 pt-1">
                                                    <p class="text-muted mb-0"><i
                                                            class="mdi mdi-phone font-size-15 align-middle pe-2 text-primary"></i>
                                                        052 6524 9896</p>
                                                    <p class="text-muted mb-0 mt-2"><i
                                                            class="mdi mdi-email font-size-15 align-middle pe-2 text-primary"></i>
                                                        KevinWest@spy.com</p>
                                                    <p class="text-muted mb-0 mt-2"><i
                                                            class="mdi mdi-google-maps font-size-15 align-middle pe-2 text-primary"></i>
                                                        88 Tadcaster PINCHBECK 6UB</p>
                                                </div>
                                                <div class="d-flex gap-2 pt-4">
                                                    <button type="button" class="btn btn-primary btn-sm w-50"><i
                                                            class="bx bx-message-square-dots me-1"></i>
                                                        Selecionar</button>
                                                </div>
                                            </div>
                                        </div>
                                    </div>
                                    <div class="col-xl-3 col-sm-6">
                                        <div class="card">
                                            <div class="card-body">
                                                <div class="d-flex align-items-center">
                                                    <div><img src="https://bootdey.com/img/Content/avatar/avatar4.png"
                                                            alt="" class="avatar-md rounded-circle img-thumbnail" />
                                                    </div>
                                                    <div class="flex-1 ms-3">
                                                        <h5 class="font-size-16 mb-1"><a href="#"
                                                                class="text-dark">Tommy Hayes</a></h5>
                                                        <span class="badge badge-soft-warning mb-0">Backend
                                                            Developer</span>
                                                    </div>
                                                </div>
                                                <div class="mt-3 pt-1">
                                                    <p class="text-muted mb-0"><i
                                                            class="mdi mdi-phone font-size-15 align-middle pe-2 text-primary"></i>
                                                        065 2563 6587</p>
                                                    <p class="text-muted mb-0 mt-2"><i
                                                            class="mdi mdi-email font-size-15 align-middle pe-2 text-primary"></i>
                                                        TommyHayes@spy.com</p>
                                                    <p class="text-muted mb-0 mt-2"><i
                                                            class="mdi mdi-google-maps font-size-15 align-middle pe-2 text-primary"></i>
                                                        5 Boar Lane SELLING 2LG</p>
                                                </div>
                                                <div class="d-flex gap-2 pt-4">
                                                    <button type="button" class="btn btn-primary btn-sm w-50"><i
                                                            class="bx bx-message-square-dots me-1"></i>
                                                        Selecionar</button>
                                                </div>
                                            </div>
                                        </div>
                                    </div>
                                    <div class="col-xl-3 col-sm-6">
                                        <div class="card">
                                            <div class="card-body">
                                                <div class="d-flex align-items-center">
                                                    <div><img src="https://bootdey.com/img/Content/avatar/avatar5.png"
                                                            alt="" class="avatar-md rounded-circle img-thumbnail" />
                                                    </div>
                                                    <div class="flex-1 ms-3">
                                                        <h5 class="font-size-16 mb-1"><a href="#"
                                                                class="text-dark">Diana Owens</a></h5>
                                                        <span class="badge badge-soft-danger mb-0">UI/UX Designer</span>
                                                    </div>
                                                </div>
                                                <div class="mt-3 pt-1">
                                                    <p class="text-muted mb-0"><i
                                                            class="mdi mdi-phone font-size-15 align-middle pe-2 text-primary"></i>
                                                        087 6321 3235</p>
                                                    <p class="text-muted mb-0 mt-2"><i
                                                            class="mdi mdi-email font-size-15 align-middle pe-2 text-primary"></i>
                                                        DianaOwens@spy.com</p>
                                                    <p class="text-muted mb-0 mt-2"><i
                                                            class="mdi mdi-google-maps font-size-15 align-middle pe-2 text-primary"></i>
                                                        52 Ilchester MYBSTER 9WX</p>
                                                </div>
                                                <div class="d-flex gap-2 pt-4">
                                                    <button type="button" class="btn btn-primary btn-sm w-50"><i
                                                            class="bx bx-message-square-dots me-1"></i>
                                                        Selecionar</button>
                                                </div>
                                            </div>
                                        </div>
                                    </div>
                                    <div class="col-xl-3 col-sm-6">
                                        <div class="card">
                                            <div class="card-body">
                                                <div class="d-flex align-items-center">
                                                    <div><img src="https://bootdey.com/img/Content/avatar/avatar6.png"
                                                            alt="" class="avatar-md rounded-circle img-thumbnail" />
                                                    </div>
                                                    <div class="flex-1 ms-3">
                                                        <h5 class="font-size-16 mb-1"><a href="#" class="text-dark">Paul
                                                                Sanchez</a></h5>
                                                        <span class="badge badge-soft-success mb-0">Full Stack
                                                            Developer</span>
                                                    </div>
                                                </div>
                                                <div class="mt-3 pt-1">
                                                    <p class="text-muted mb-0"><i
                                                            class="mdi mdi-phone font-size-15 align-middle pe-2 text-primary"></i>
                                                        021 0125 5689</p>
                                                    <p class="text-muted mb-0 mt-2"><i
                                                            class="mdi mdi-email font-size-15 align-middle pe-2 text-primary"></i>
                                                        DianaOwens@spy.com</p>
                                                    <p class="text-muted mb-0 mt-2"><i
                                                            class="mdi mdi-google-maps font-size-15 align-middle pe-2 text-primary"></i>
                                                        80 South Street MONKW 7BR</p>
                                                </div>
                                                <div class="d-flex gap-2 pt-4">
                                                    <button type="button" class="btn btn-primary btn-sm w-50"><i
                                                            class="bx bx-message-square-dots me-1"></i>
                                                        Selecionar</button>
                                                </div>
                                            </div>
                                        </div>
                                    </div>
                                </div>
                                <div class="row g-0 align-items-center pb-4">
                                    <div class="col-sm-11">
                                        <div class="float-sm-end">
                                            <nav aria-label="...">
                                                <ul class="pagination pagination-sm">
                                                    <li class="page-item active" aria-current="page">
                                                        <span class="page-link">1</span>
                                                    </li>
                                                    <li class="page-item"><a class="page-link" href="#">2</a></li>
                                                    <li class="page-item"><a class="page-link" href="#">3</a></li>
                                                </ul>
                                            </nav>
                                        </div>
                                    </div>
                                </div>
                            </div>
                            <div class="modal-footer">
                                <button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Fechar</button>
                            </div>
                        </div>
                    </div>
                </div>

    </section>



    <!-- ===== IONICONS ===== -->
    <script src="https://unpkg.com/ionicons@5.1.2/dist/ionicons.js"></script>

    <!-- ===== MAIN JS ===== -->
    <script src="assets/js/main.js"></script>

    <!-- ===== BOOTSTRAP ===== -->
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.bundle.min.js"
        integrity="sha384-C6RzsynM9kWDrMNeT87bh95OGNyZPhcTNXj1NW7RuBCsyN/o0jlpcV8Qyq46cDfL"
        crossorigin="anonymous"></script>
</body>

</html>
------------------ login.html-------------------
<!DOCTYPE html>
<html lang="br">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/css/bootstrap.min.css" rel="stylesheet"
        integrity="sha384-T3c6CoIi6uLrA9TneNEoa7RxnatzjcDSCmG1MXxSR1GAsXEV/Dwwykc2MPK8M2HN" crossorigin="anonymous">
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.bundle.min.js"
        integrity="sha384-C6RzsynM9kWDrMNeT87bh95OGNyZPhcTNXj1NW7RuBCsyN/o0jlpcV8Qyq46cDfL"
        crossorigin="anonymous"></script>
    <script src="assets/js/main.js"></script>
        
    <link rel="stylesheet" href="assets/css/login.css">
    <title>Login</title>
</head>

<body>
    <div class="container">
        <div class="row">
            <div class="col-lg-3 col-md-2"></div>
            <div class="col-lg-6 col-md-8 login-box">
                <div class="col-lg-12 login-key">
                    <img class="login-image" src="assets/img/logo_monitoria.png" alt="">
                </div>
                <div class="col-lg-12 login-title">
                    Login de Usuário
                </div>

                <div class="col-lg-12 login-form">
                    <div class="col-lg-12 login-form">
                        <form>
                            <div class="form-group">
                                <label class="form-control-label">Usuário</label>
                                <input type="text" class="form-control" id="email" placeholder="e-mail">
                            </div>
                            <div class="form-group">
                                <label class="form-control-label">Senha</label>
                                <input type="password" class="form-control" id="senha" placeholder="senha">
                            </div>

                            <div class="col-lg-12 loginbttm">
                                <div class="col-lg-6 forgot-password">
                                    <p><a href="#" class="text-primary">Esqueceu sua senha?</a></p>
                                </div>
                                <div class="col-lg-6 check-box">
                                    <label class="form-check-label">
                                        <input class="form-check-input" type="checkbox" name="remember"> Lembre-se de
                                        mim
                                    </label>
                                </div>
                                <div class="radio-box">
                                    <div class="form-check">
                                        <input class="form-check-input" type="radio"value="aluno" name="flexRadioDefault"
                                            id="flexRadioDefault1">
                                        <label class="form-check-label" for="flexRadioDefault1">
                                            Aluno
                                        </label>
                                    </div>
                                    <div class="form-check">
                                        <input class="form-check-input" type="radio" name="flexRadioDefault"
                                            id="flexRadioDefault2" value="mentor" checked>
                                        <label class="form-check-label" for="flexRadioDefault2">
                                            Mentor
                                        </label>
                                    </div>
                                    <div class="form-check">
                                        <input class="form-check-input" type="radio" value="professor" name="flexRadioDefault"
                                            id="flexRadioDefault3" checked>
                                        <label class="form-check-label" for="flexRadioDefault3">
                                            Professor
                                        </label>
                                    </div>
                                </div>
                                <div class="col-lg-6 login-btm login-button">
                                    <a class="btn btn-outline-primary" onclick="logar()">LOGIN</a>

                                </div>
                            </div>
                        </form>
                    </div>
                </div>
                <div class="col-lg-3 col-md-2"></div>
            </div>
        </div>
</body>

</html>

------------------ mensagem.html-------------------
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <!-- ===== BOOTSTRAP ===== -->
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/css/bootstrap.min.css" rel="stylesheet"
        integrity="sha384-T3c6CoIi6uLrA9TneNEoa7RxnatzjcDSCmG1MXxSR1GAsXEV/Dwwykc2MPK8M2HN" crossorigin="anonymous">
    <!-- ===== CSS ===== -->
    <link rel="stylesheet" href="assets/css/styles.css">
    <!-- ===== ICON ===== -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.2/css/all.min.css"
        integrity="sha512-z3gLpd7yknf1YoNbCzqRKc4qyor8gaKU1qmn+CShxbuBusANI9QpRohGBreCFkKxLhei6S9CQXFEbbKuqLg0DA=="
        crossorigin="anonymous" referrerpolicy="no-referrer" />

    <script src="https://code.jquery.com/jquery-3.5.1.slim.min.js"></script>
    <script src="https://cdn.jsdelivr.net/npm/@popperjs/core@2.9.3/dist/umd/popper.min.js"></script>

    <title>PUC Minas - Programa de Monitoria</title>
</head>

<body id="body-pd">
    <div class="l-navbar" id="navbar">
        <nav class="nav">
            <div>
                <div class="nav__brand">
                    <ion-icon name="menu-outline" class="nav__toggle" id="nav-toggle"></ion-icon>
                    <a href="mensagem.html" class="nav__logo"><img id="logo" src="assets/img/logo.png"
                            width="15%"></a>
                </div>

                <div class="nav__list">
                    <a href="painel_aluno.html" class="nav__link active">
                        <ion-icon name="home-outline" class="nav__icon"></ion-icon>
                        <span class="nav__name">Painel de Controle</span>
                    </a>

                    <a href="mensagem.html" class="nav__link">
                        <ion-icon name="chatbubbles-outline" class="nav__icon"></ion-icon>
                        <span class="nav__name">Mensagem</span>
                    </a>

                    <a href="agenda.html" class="nav__link">
                        <ion-icon name="calendar-outline" class="nav__icon"></ion-icon>
                        <span class="nav__name">Calendario</span>
                    </a>

                    <a href="https://teams.microsoft.com/dl/launcher/launcher.html?url=teams&type=meetup-join&enableMobilePage=true&suppressPrompt=true&tenantId=14cbd5a7-ec94-46ba-b314-cc0fc972a161"
                        class="nav__link">
                        <ion-icon name="tv" class="nav__icon"></ion-icon>
                        <span class="nav__name">Teams</span>
                    </a>


                    <a href="ajuda.html" class="nav__link">
                        <ion-icon name="help-outline" class="nav__icon"></ion-icon>
                        <span class="nav__name">Ajuda</span>
                    </a>

                    <a href="config.html" class="nav__link">
                        <ion-icon name="settings-outline" class="nav__icon"></ion-icon>
                        <span class="nav__name">Configurações</span>
                    </a>
                </div>
            </div>



            <div>
                <img id="foto" src="assets/img/foto.png" width="12%">
            </div>

            <a href="login.html" class="nav__link">
                <ion-icon name="log-out-outline" class="nav__icon"></ion-icon>
                <span class="nav__name">Sair</span>
            </a>
        </nav>
    </div>

    <section class="container-fluid">
        <div class="row">
            <div class="col-md-10">
                <div class="border-bottom" class="titulo">
                    <h1>Caixa de Entrada</h1>
                </div>
            </div>
            <div class="col-2">
                <div>
                    <a href="login.html">
                        <button type="button" class="btn btn-dark"><i class="fa-solid fa-right-from-bracket"></i>
                            Sair</button>
                    </a>
                </div>
            </div>
        </div>

        <div class="row">
            <div class="col-md-2 pt-2">
                <link href="https://maxcdn.bootstrapcdn.com/font-awesome/4.3.0/css/font-awesome.min.css"
                    rel="stylesheet">
                <button type="button" class="btn btn-primary" data-bs-toggle="modal" data-bs-target="#modal1">
                    Enviar Mensagem
                </button>
                <hr>
                <div>
                    <ul>
                        <li class="header"><strong>Pastas</strong></li>
                        <li><a href="mensagem.html"><i class="fa fa-envelope"></i> Caixa de Entrada</a></li>
                        <li><a href="caixadesaida.html"><i class="fa fa-envelope-o"></i> Caixa de Saída</a></li>
                        <li><a href="importantes.html"><i class="fa fa-bookmark"></i> Importantes</a></li>
                        <li><a href="Lixeira.html"><i class="fa fa-pencil-square-o"></i> Lixeira</a></li>
                    </ul>
                </div>
            </div>

            <!-- BEGIN INBOX CONTENT -->
            <div class="col-md-9">
                <div class="row">
                    <div class="col-sm-6">
                        <label style="margin-right: 8px;" class="">
                            <div class="icheckbox_square-blue" style="position: relative;"><input type="checkbox"
                                    id="check-all" class="icheck"
                                    style="position: absolute; top: -20%; left: -20%; display: block; width: 140%; height: 140%; margin: 0px; padding: 0px; border: 0px; opacity: 0; background: rgb(255, 255, 255);"><ins
                                    class="iCheck-helper"
                                    style="position: absolute; top: -20%; left: -20%; display: block; width: 140%; height: 140%; margin: 0px; padding: 0px; border: 0px; opacity: 0; background: rgb(255, 255, 255);"></ins>
                            </div>
                        </label>
                        <div class="btn-group pt-4">
                            <button type="button" class="btn btn-default dropdown-toggle" data-toggle="dropdown">
                                Filtro <span class="caret"></span>
                            </button>
                            <ul class="dropdown-menu" role="menu">
                                <li><a href="mensagem.html">Mark as read</a></li>
                                <li><a href="caixadesaida.html">Mark as unread</a></li>
                                <li><a href="importantes.htm">Mark as important</a></li>
                                <li><a href="Lixeira.html">Delete</a></li>
                            </ul>
                        </div>
                    </div>

                    <div class="col-md-6 search-form pt-2 pb-2 ">
                        <form action="#" class="text-right">
                            <div class="input-group">
                                <form class="d-flex" role="search">
                                    <input class="form-control me-2" type="search" placeholder="Pesquisar"
                                        aria-label="Search" id="searchInput">
                                    <button class="btn btn-outline-success" type="submit">Pesquisar</button>
                                </form>
                        </form>
                    </div>
                </div>

                <div class="padding"></div>

                <div class="table-responsive ">
                    <table class="table">
                        <tbody>
                            <tr id="message1">
                                <td class="action"><input type="checkbox" /></td>
                                <td class="action"><i class="fa fa-bookmark-o"></i></td>
                                <td class="name"><a href="#" data-bs-toggle="modal" data-bs-target="#modal2">Mateus
                                        oliveira
                                    </a></td>
                                <td class="subject"><a href="#" data-bs-toggle="modal" data-bs-target="#modal2"> Olá,
                                        mentor! Tenho enfrentado algumas dificuldades com... </a></td>
                                <td class="time">08:30 PM</td>
                            </tr>
                        </tbody>
                    </table>
                </div>

                <nav>
                    <ul class="pagination">
                        <li class="page-item">
                            <a class="page-link" href="#">Voltar</a>
                        </li>
                        <li class="page-item"><a class="page-link" href="#">1</a></li>
                        <li class="page-item" aria-current="page">
                            <a class="page-link" href="#">2</a>
                        </li>
                        <li class="page-item"><a class="page-link" href="#">3</a></li>
                        <li class="page-item">
                            <a class="page-link" href="#">Proxima</a>
                        </li>
                    </ul>
                </nav>
                <!-- END INBOX CONTENT -->
                <script>
                    $(document).ready(function () {
                        $('#searchInput').on('input', function () {
                            var searchTerm = $(this).val().toLowerCase();

                            $('tbody tr').each(function () {
                                var name = $(this).find('.name a').text().toLowerCase();
                                var subject = $(this).find('.subject a').text().toLowerCase();

                                var match = name.includes(searchTerm) || subject.includes(searchTerm);

                                $(this).toggle(match);
                            });
                        });
                    });
                </script>

            </div>
        </div>



        <!-- Modal 1 -->
        <div class="modal fade" id="modal1" tabindex="-1" aria-labelledby="exampleModalLabel" aria-hidden="true">
            <div class="modal-dialog">
                <div class="modal-content">
                    <div class="modal-header">
                        <h1 class="modal-title fs-5" id="exampleModalLabel">Nova mensagem</h1>

                        
                        <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
                    </div>
                    <div class="modal-body">
                        <main>
                            <div class="panel-body contacts">
                                <button type="button" class="btn btn-primary" data-bs-toggle="modal"
                                    data-bs-target="#modal3"><i class="fa-solid fa-address-book"></i>
                                    Contatos
                                </button>
                            </div>
                            <form>
                                <div class="form-row mb-3">
                                    <label for="to" class="col-2 col-sm-1 col-form-label">Para:</label>
                                    <div class="col-10 col-sm-11">
                                        <input type="email" class="form-control" id="to" placeholder="email">
                                    </div>
                                </div>
                                <div class="form-row mb-3">
                                    <label for="cc" class="col-2 col-sm-1 col-form-label">Assunto:</label>
                                    <div class="col-10 col-sm-11">
                                        <input type="email" class="form-control" id="cc" placeholder="assunto">
                                    </div>
                                </div>

                                <div class="form-row mb-3">
                                    <label for="cc" class="col-2 col-sm-1 col-form-label">CC:</label>
                                    <div class="col-10 col-sm-11">
                                        <input type="email" class="form-control" id="cc" placeholder="copias">
                                    </div>
                                </div>

                            </form>
                            <div class="row">
                                <div class="col-sm-11 ml-auto">
                                    <div class="toolbar" role="toolbar">
                                        <div class="btn-group">
                                            <button type="button" class="btn btn-light">
                                                <span class="fa fa-bold"></span>
                                            </button>
                                            <button type="button" class="btn btn-light">
                                                <span class="fa fa-italic"></span>
                                            </button>
                                            <button type="button" class="btn btn-light">
                                                <span class="fa fa-underline"></span>
                                            </button>
                                        </div>

                                        <button type="button" class="btn btn-light">
                                            <span class="fa fa-trash-o"></span>
                                        </button>
                                        <button type="button" class="btn btn-light">
                                            <span class="fa fa-paperclip"></span>
                                        </button>
                                    </div>
                                    <div class="form-group mt-4">
                                        <textarea class="form-control" id="message" name="body" rows="12"
                                            placeholder="escrever"></textarea>
                                    </div>
                                    <div class="form-group mt-4">
                                        <button type="submit" class="btn btn-danger"
                                            data-bs-dismiss="modal">Cancelar</button>
                                        <button type="submit" class="btn btn-success">Enviar</button>
                                    </div>
                                </div>
                            </div>
                        </main>
                    </div>
                    <div class="modal-footer">
                        <button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Fechar</button>
                    </div>
                </div>
            </div>

            

            <script>
                document.addEventListener('DOMContentLoaded', function () {
                    document.querySelector('#modal1 .btn-success').addEventListener('click', function () {
                        alert('Mensagem enviada com sucesso!');
                        $('#modal1').modal('hide');
                    });
                });
            </script>
        </div>
        <!-- Modal 1 FIM -->

        <!-- Modal 2 -->
        <div class="modal fade" id="modal2" tabindex="-1" aria-labelledby="exampleModalLabel" aria-hidden="true">
            <div class="modal-dialog">
                <div class="modal-content">
                    <div class="modal-header">
                        <h1 class="modal-title fs-5" id="exampleModalLabel">Caixa de entrada</h1>
                        <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
                    </div>
                    <div class="modal-body">
                        <main>
                            <link href="https://maxcdn.bootstrapcdn.com/font-awesome/4.3.0/css/font-awesome.min.css"
                                rel="stylesheet">
                            <div class="container">
                                <div class="row inbox">
                                    <div class="col-md-3">
                                        <div class="panel panel-default">
                                            <div class="panel-body inbox-menu">
                                                <a href="#" data-bs-toggle="modal" data-bs-target="#modal1"
                                                    class="btn btn-danger btn-block">Enviar Mensagem </a>
                                                <ul>
                                                    <li>
                                                        <a href="mensagem.html"><i class="fa fa-inbox"></i> Caixa de
                                                            Entrada <span class="label label-danger"></span></a>
                                                    </li>
                                                    <li>
                                                        <a href="caixadesaida.html"><i class="fa fa-rocket"></i> Caixa
                                                            de Saída</a>
                                                    </li>
                                                    <li>
                                                        <a href="Lixeira.html"><i class="fa fa-trash-o"></i> Lixo</a>
                                                    </li>
                                                    <li>
                                                        <a href="importantes.html"><i class="fa fa-bookmark"></i>
                                                            Importantes<span class="label label-info"></span></a>
                                                    </li>
                                                    <li class="title">
                                                </ul>
                                            </div>
                                        </div>
                                        <div class="panel panel-default">
                                            <div class="panel-body contacts">
                                                <button type="button" class="btn btn-primary" data-bs-toggle="modal"
                                                    data-bs-target="#modal3"><i class="fa-solid fa-address-book"></i>
                                                    Contatos
                                                </button>
                                            </div>
                                        </div>
                                    </div><!--/.col-->
                                    <div class="col-md-9">
                                        <div class="panel panel-default">
                                            <div class="panel-body message">
                                                <span class="btn-group">

                                                    <button id="importantBtn" class="btn btn-default"><span
                                                            class="fa fa-bookmark-o"></span></button>
                                                </span>
                                                <span class="btn-group">
                                                    <button class="btn btn-default"><span
                                                            class="fa fa-mail-reply"></span></button>
                                                    <button class="btn btn-default"><span
                                                            class="fa fa-mail-reply-all"></span></button>
                                                    <button class="btn btn-default"><span
                                                            class="fa fa-mail-forward"></span></button>
                                                </span>
                                                <button id="trashBtn" class="btn btn-default"><span
                                                        class="fa fa-trash-o"></span></button>

                                                <div class="message-title">Dificuldade em Switch </div>
                                                <div class="header">
                                                    <img class="avatar"
                                                        src="https://bootdey.com/img/Content/avatar/avatar1.png">
                                                    <div class="from">
                                                        <span>Mateus oliveira</span>
                                                        mateus.oliveira2121@gmail.com
                                                    </div>
                                                    <div class="date"><span class="fa fa-paper-clip"></span> Today,
                                                        <b>3:47 PM</b>
                                                    </div>
                                                    <div class="menu"></div>
                                                </div>
                                                <div class="content">
                                                    <p>
                                                        Olá, mentor! Tenho enfrentado algumas dificuldades com a
                                                        programação em C#. Sinto que preciso de ajuda para entender
                                                        melhor os conceitos de switch. Será que você pode me orientar?
                                                    </p>
                                                    <blockquote>
                                                        <!---->
                                                    </blockquote>
                                                </div>
                                                <div class="attachments">
                                                    <ul>
                                                        <li>
                                                            <span class="label label-danger">zip</span>
                                                            <b>bootstrap.zip</b> <i>(2,5MB)</i>
                                                            <span class="quickMenu">
                                                                <a href="#" class="fa fa-search"><i></i></a>
                                                                <a href="#" class="fa fa-share"><i></i></a>
                                                                <a href="#" class="fa fa-cloud-download"><i></i></a>
                                                            </span>
                                                        </li>
                                                        <li>
                                                            <span class="label label-info">txt</span> <b>readme.txt</b>
                                                            <i>(7KB)</i>
                                                            <span class="quickMenu">
                                                                <a href="#" class="fa fa-search"><i></i></a>
                                                                <a href="#" class="fa fa-share"><i></i></a>
                                                                <a href="#" class="fa fa-cloud-download"><i></i></a>
                                                            </span>
                                                        </li>
                                                        <li>
                                                            <span class="label label-success">xls</span>
                                                            <b>spreadsheet.xls</b> <i>(984KB)</i>
                                                            <span class="quickMenu">
                                                                <a href="#" class="fa fa-search"><i></i></a>
                                                                <a href="#" class="fa fa-share"><i></i></a>
                                                                <a href="#" class="fa fa-cloud-download"><i></i></a>
                                                            </span>
                                                        </li>
                                                    </ul>
                                                </div>
                                                <form method="post" action="">
                                                    <div class="form-group">
                                                        <textarea class="form-control" id="message" name="body"
                                                            rows="12" placeholder="escreva"></textarea>
                                                    </div>
                                                    <div class="form-group pt-2">
                                                        <button tabindex="3" type="submit"
                                                            class="btn btn-success">Responder</button>
                                                    </div>
                                                </form>
                                            </div>
                                        </div>
                                    </div><!--/.col-->
                                </div>
                            </div>
                        </main>
                    </div>
                    <div class="modal-footer">
                        <button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Fechar</button>
                    </div>
                </div>
            </div>

            <script>
                document.addEventListener('DOMContentLoaded', function () {
                    document.querySelector('#importantBtn').addEventListener('click', function () {

                        alert('Email marcado como importante.');

                        $('#modal2').modal('hide');
                    });
                });
            </script>

            <script>
                document.addEventListener('DOMContentLoaded', function () {
                    document.querySelector('#trashBtn').addEventListener('click', function () {

                        alert('Email movido para a Lixeira.');

                        $('#modal2').modal('hide');
                    });
                });
            </script>

            <script>
                document.addEventListener('DOMContentLoaded', function () {
                    document.querySelector('#modal2 .btn-success').addEventListener('click', function (event) {
                        event.preventDefault();

                        alert('Mensagem enviada com sucesso!');

                        $('#modal2').modal('hide');
                    });
                });
            </script>
        </div>
        <!-- Modal 2 FIM -->

        <!-- Modal 3 -->
        <div class="modal fade" id="modal3" tabindex="-1" aria-labelledby="exampleModalLabel" aria-hidden="true">
            <div class="modal-dialog">
                <div class="modal-content">
                    <div class="modal-header">
                        <h1 class="modal-title fs-5" id="exampleModalLabel">Contatos</h1>
                        <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
                    </div>
                    <div class="modal-body">
                        <div class="container">
                            <div class="row align-items-center">
                                <div class="row" id="respostaRequisicao"></div>

                                <script>
                                    document.addEventListener('DOMContentLoaded', function () {
                                        // URL da sua API para buscar os dados do contato (substitua pelo seu URL real)
                                        var apiUrl = 'https://db.samuelcorreia4.repl.co/usuarios';

                                        // Realiza a requisição à API usando o fetch
                                        fetch(apiUrl)
                                            .then(response => response.json())
                                            .then(data => {
                                                // Manipula os dados recebidos e preenche a div com a resposta da requisição

                                                // Seleciona a div de resposta
                                                var respostaDiv = document.getElementById('respostaRequisicao');

                                                // Loop através dos contatos e cria os elementos HTML
                                                data.forEach(contact => {
                                                    // Cria um novo elemento de card para cada contato
                                                    var cardElement = document.createElement('div');
                                                    cardElement.className = 'col-xl-3 col-sm-6';

                                                    cardElement.innerHTML = `
                                                <div class="card">
                                                    <div class="card-body">
                                                        <div class="d-flex align-items-center">
                                                            <div>
                                                                <img src="${contact.foto}" alt="" class="avatar-md rounded-circle img-thumbnail" />
                                                            </div>
                                                            <div class="flex-1 ms-3">
                                                                <h5 class="font-size-16 mb-1"><a href="#" class="text-dark">${contact.usuario}</a></h5>
                                                            </div>
                                                        </div>
                                                        <div class="mt-3 pt-1">
                                                            <p class="text-muted mb-0"><i class="mdi mdi-phone font-size-15 align-middle pe-2 text-primary"></i>${contact.telefone}</p>
                                                            <p class="text-muted mb-0 mt-2"><i class="mdi mdi-email font-size-15 align-middle pe-2 text-primary"></i>${contact.email}</p>
                                                        </div>
                                                        <div class="d-flex gap-2 pt-4">
                                                            <button type="button" class="btn btn-primary btn-sm w-50" onclick="selecionarContato('${contact.usuario}', '${contact.telefone}', '${contact.email}')" data-bs-dismiss="modal"><i class="bx bx-message-square-dots me-1"></i>Selecionar</button>
                                                        </div>
                                                    </div>
                                                </div>
                                            `;

                                                    // Adiciona o novo card à div de resposta
                                                    respostaDiv.appendChild(cardElement);
                                                });
                                            })
                                            .catch(error => console.error('Erro na requisição:', error));

                                        // Função para preencher o Modal 1 com as informações do contato selecionado
                                        window.selecionarContato = function (nome, telefone, email) {
                                            document.getElementById('to').value = email;
                                            document.getElementById('cc').value = '';  // Limpar o campo CC
                                            document.getElementById('message').value = `Olá ${nome},\n\n`;  // Mensagem inicial
                                            $('#modal1').modal('show');  // Exibir o Modal 1
                                        };
                                    });
                                </script>
                            </div>
                            <div class="modal-footer">
                                <button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Fechar</button>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>



    </section>



    <!-- ===== IONICONS ===== -->
    <script src="https://unpkg.com/ionicons@5.1.2/dist/ionicons.js"></script>

    <!-- ===== MAIN JS ===== -->
    <script src="assets/js/main.js"></script>

    <!-- ===== BOOTSTRAP ===== -->
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.bundle.min.js"
        integrity="sha384-C6RzsynM9kWDrMNeT87bh95OGNyZPhcTNXj1NW7RuBCsyN/o0jlpcV8Qyq46cDfL"
        crossorigin="anonymous"></script>
</body>

</html>

------------------ painel_aluno.html-------------------
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/css/bootstrap.min.css" rel="stylesheet"
        integrity="sha384-T3c6CoIi6uLrA9TneNEoa7RxnatzjcDSCmG1MXxSR1GAsXEV/Dwwykc2MPK8M2HN" crossorigin="anonymous">

    <!-- ===== CSS ===== -->
    <link rel="stylesheet" href="assets/css/styles.css">

    <title>PUC Minas - Programa de Monitoria</title>
</head>

<body id="body-pd">
    <div class="l-navbar" id="navbar">
        <nav class="nav">
            <div>
                <div class="nav__brand">
                    <ion-icon name="menu-outline" class="nav__toggle" id="nav-toggle"></ion-icon>
                    <a href="painel_aluno.html" class="nav__logo"><img id="logo" src="assets/img/logo.png"
                            width="15%"></a>
                </div>

                <div class="nav__list">
                    <a href="painel_aluno.html" class="nav__link active">
                        <ion-icon name="home-outline" class="nav__icon"></ion-icon>
                        <span class="nav__name">Painel de Controle</span>
                    </a>

                    <a href="mensagem.html" class="nav__link">
                        <ion-icon name="chatbubbles-outline" class="nav__icon"></ion-icon>
                        <span class="nav__name">Mensagem</span>
                    </a>

                    <a href="agenda.html" class="nav__link">
                        <ion-icon name="calendar-outline" class="nav__icon"></ion-icon>
                        <span class="nav__name">Calendario</span>
                    </a>

                    <a href="https://teams.microsoft.com/dl/launcher/launcher.html?url=teams&type=meetup-join&enableMobilePage=true&suppressPrompt=true&tenantId=14cbd5a7-ec94-46ba-b314-cc0fc972a161"
                        class="nav__link">
                        <ion-icon name="tv" class="nav__icon"></ion-icon>
                        <span class="nav__name">Teams</span>
                    </a>


                    <a href="ajuda.html" class="nav__link">
                        <ion-icon name="help-outline" class="nav__icon"></ion-icon>
                        <span class="nav__name">Ajuda</span>
                    </a>

                    <a href="config.html" class="nav__link">
                        <ion-icon name="settings-outline" class="nav__icon"></ion-icon>
                        <span class="nav__name">Configurações</span>
                    </a>
                </div>
            </div>



            <div>
                <img id="foto" src="assets/img/foto.png" width="15%">
            </div>



            <a href="login.html" class="nav__link">
                <ion-icon name="log-out-outline" class="nav__icon"></ion-icon>
                <span class="nav__name">Sair</span>
            </a>
        </nav>
    </div>

    <section class="container-fluid">
        <div class="row">
            <div class="col-md-12">
                <div class="border-bottom" class="titulo">
                    <h1>Painel de controle</h1>
                </div>
                <div class="row">
                    <div class="col-md-3 pt-4">
                        <div class="card-deck">
                            <div class="card">
                                <img src="assets/img/DWnovo.png.gif" class="card-img-top" alt="ONG 1">
                                <div class="card-body">
                                    <h5 class="card-title">Introdução a Computação</h5>
                                    <a href="IC_aluno.html"
                                        class="btn btn-primary">Acessar</a>
                                </div>
                            </div>
                        </div>
                    </div>

                    <div class="col-md-3 pt-4">
                        <div class="card-deck">
                            <div class="card">
                                <img src="assets/img/mobile.png" class="card-img-top" alt="ONG 2">
                                <div class="card-body">
                                    <h5 class="card-title">Trabalho interdisciplinar</h5>
                                    <a href="TIAW_aluno.html"
                                        class="btn btn-primary">Acessar</a>
                                </div>
                            </div>
                        </div>
                    </div>

                    <div class="col-md-3 pt-4">
                        <div class="card-deck">
                            <div class="card">
                                <img src="assets/img/agoritmo.png" class="card-img-top" alt="ONG 3">
                                <div class="card-body">
                                    <h5 class="card-title">Algoritmos e Programação</h5>
                                    <a href="ATP_aluno.html" class="btn btn-primary">Acessar</a>
                                </div>
                            </div>
                        </div>
                    </div>

                </div>
            </div>
    </section>



    <!-- ===== IONICONS ===== -->
    <script src="https://unpkg.com/ionicons@5.1.2/dist/ionicons.js"></script>

    <!-- ===== MAIN JS ===== -->
    <script src="assets/js/main.js"></script>

    <!-- ===== BOOTSTRAP ===== -->
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.bundle.min.js"
        integrity="sha384-C6RzsynM9kWDrMNeT87bh95OGNyZPhcTNXj1NW7RuBCsyN/o0jlpcV8Qyq46cDfL"
        crossorigin="anonymous"></script>

</body>

</html>
------------------painel_monitor.html-------------------
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/css/bootstrap.min.css" rel="stylesheet"
        integrity="sha384-T3c6CoIi6uLrA9TneNEoa7RxnatzjcDSCmG1MXxSR1GAsXEV/Dwwykc2MPK8M2HN" crossorigin="anonymous">

    <!-- ===== CSS ===== -->
    <link rel="stylesheet" href="assets/css/styles.css">
    <!-- ===== ICON ===== -->
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.2/css/all.min.css"
  integrity="sha512-z3gLpd7yknf1YoNbCzqRKc4qyor8gaKU1qmn+CShxbuBusANI9QpRohGBreCFkKxLhei6S9CQXFEbbKuqLg0DA=="
  crossorigin="anonymous" referrerpolicy="no-referrer" />

    <title>PUC Minas - Programa de Monitoria</title>
</head>

<body id="body-pd">
    <div class="l-navbar" id="navbar">
        <nav class="nav">
            <div>
                <div class="nav__brand">
                    <ion-icon name="menu-outline" class="nav__toggle" id="nav-toggle"></ion-icon>
                    <a href="painel_monitor.html" class="nav__logo"><img id="logo" src="assets/img/logo.png"
                            width="15%"></a>
                </div>

                <div class="nav__list">
                    <a href="painel_monitor.html" class="nav__link active">
                        <ion-icon name="home-outline" class="nav__icon"></ion-icon>
                        <span class="nav__name">Painel do Monitor</span>
                    </a>

                    <a href="mensagem.html" class="nav__link">
                        <ion-icon name="chatbubbles-outline" class="nav__icon"></ion-icon>
                        <span class="nav__name">Mensagem</span>
                    </a>

                    <a href="agenda.html" class="nav__link">
                        <ion-icon name="calendar-outline" class="nav__icon"></ion-icon>
                        <span class="nav__name">Calendario</span>
                    </a>

                    <a href="https://teams.microsoft.com/dl/launcher/launcher.html?url=teams&type=meetup-join&enableMobilePage=true&suppressPrompt=true&tenantId=14cbd5a7-ec94-46ba-b314-cc0fc972a161"
                        class="nav__link">
                        <ion-icon name="tv" class="nav__icon"></ion-icon>
                        <span class="nav__name">Teams</span>
                    </a>


                    <a href="ajuda.html" class="nav__link">
                        <ion-icon name="help-outline" class="nav__icon"></ion-icon>
                        <span class="nav__name">Ajuda</span>
                    </a>

                    <a href="config.html" class="nav__link">
                        <ion-icon name="settings-outline" class="nav__icon"></ion-icon>
                        <span class="nav__name">Configurações</span>
                    </a>
                </div>
            </div>



            <div>
                <img id="foto" src="assets/img/foto.png" width="15%">
            </div>



            <a href="login.html" class="nav__link">
                <ion-icon name="log-out-outline" class="nav__icon"></ion-icon>
                <span class="nav__name">Sair</span>
            </a>
        </nav>
    </div>

    <!-- Modal -->
    <div class="modal fade" id="add_conteudo" tabindex="-1" aria-labelledby="exampleModalLabel" aria-hidden="true">
        <div class="modal-dialog">
            <div class="modal-content">
                <div class="modal-header">
                    <h1 class="modal-title fs-5" id="exampleModalLabel"><i class="fa-regular fa-file"></i> Adicionar Novo Conteúdo</h1>
                    <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
                </div>
                <div class="modal-body">
                    <form action="/salvar-conteudo" method="post">
                        <div class="form-group">
                            <label for="titulo">Digite o título da Semana:</label>
                            <input type="text" class="form-control" id="titulo" name="titulo">
                        </div>

                        <div class="form-group">
                            <label for="texto">Digite seu texto:</label>
                            <textarea class="form-control" id="texto" name="texto" rows="4"></textarea>
                        </div>

                        <div class="form-group">
                            <label for="video"><i class="fa-solid fa-video"></i> Adicionar Mídia</label>
                            <input type="file" class="form-control-file" id="video" name="video" accept="video/*">
                        </div>
                    </form>
                </div>
                <div class="modal-footer">
                    <button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Cancelar</button>
                    <button type="button" class="btn btn-primary">Concluir</button>
                </div>
            </div>
        </div>
    </div>

    <section class="container-fluid">
        <div class="row">
            <div class="col-md-12">
                <div class="border-bottom" class="titulo">
                    <h1>Painel do Monitor</h1>
                </div>
                <div class="row">
                    <div class="col-md-3 pt-4">
                        <div class="card-deck">
                            <div class="card">
                                <img src="assets/img/DWnovo.png.gif" class="card-img-top" alt="ONG 1">
                                <div class="card-body">
                                    <h5 class="card-title">Introdução a Computação</h5>
                                    <div class="row">
                                        <div class="col-4">
                                            <label for="imagem" style="margin-bottom: 1%;">Imagem:</label>
                                            <label for="upload" class="btn btn-primary me-2 mb-4" tabindex="0">
                                                <span class="d-none d-sm-block">Carregar</span>
                                                <i class="bx bx-upload d-block d-sm-none"></i>
                                                <input type="file" id="upload" class="account-file-input" hidden accept="image/png, image/jpeg" />
                                              </label>
                                        </div>
                                    </div>
                                    <p class="text-muted mb-0" style="margin-top: -7%;">Formatos permitidos JPG, GIF ou PNG</p>
                                    <a href="IC_Monitor.html" class="btn btn-primary" style="margin-top: 2%;">Acessar</a>
                                    <button type="button" class="btn btn-success" data-bs-toggle="modal" style="margin-top: 2%;"
                                        data-bs-target="#add_conteudo">
                                        Adicionar Conteudo
                                    </button>
                                </div>
                            </div>
                        </div>
                    </div>

                    <div class="col-md-3 pt-4">
                        <div class="card-deck">
                            <div class="card">
                                <img src="assets/img/mobile.png" class="card-img-top" alt="ONG 2">
                                <div class="card-body">
                                    <h5 class="card-title">Trabalho interdisciplinar</h5>
                                    <div class="row">
                                        <div class="col-4">
                                            <label for="imagem" style="margin-bottom: 1%;">Imagem:</label>
                                            <label for="upload" class="btn btn-primary me-2 mb-4" tabindex="0">
                                                <span class="d-none d-sm-block">Carregar</span>
                                                <i class="bx bx-upload d-block d-sm-none"></i>
                                                <input type="file" id="upload" class="account-file-input" hidden accept="image/png, image/jpeg" />
                                              </label>
                                        </div>
                                    </div>
                                    <p class="text-muted mb-0" style="margin-top: -7%;">Formatos permitidos JPG, GIF ou PNG</p>
                                    <a href="TIAW_Monitor.html" class="btn btn-primary" style="margin-top: 2%;">Acessar</a>
                                    <button type="button" class="btn btn-success" style="margin-top: 2%;" data-bs-toggle="modal"
                                        data-bs-target="#add_conteudo">
                                        Adicionar Conteudo
                                    </button>
                                </div>
                            </div>
                        </div>
                    </div>

                    <div class="col-md-3 pt-4">
                        <div class="card-deck">
                            <div class="card">
                                <img src="assets/img/agoritmo.png" class="card-img-top" alt="ONG 3">
                                <div class="card-body">
                                    <h5 class="card-title">Algoritmos e Programação</h5>
                                    <div class="row">
                                        <div class="col-4">
                                            <label for="imagem" style="margin-bottom: 1%;">Imagem:</label>
                                            <label for="upload" class="btn btn-primary me-2 mb-4" tabindex="0">
                                                <span class="d-none d-sm-block">Carregar</span>
                                                <i class="bx bx-upload d-block d-sm-none"></i>
                                                <input type="file" id="upload" class="account-file-input" hidden accept="image/png, image/jpeg" />
                                              </label>
                                        </div>
                                    </div>
                                    <p class="text-muted mb-0" style="margin-top: -7%;">Formatos permitidos JPG, GIF ou PNG</p>
                                    <a href="ATP_Monitor.html" class="btn btn-primary" style="margin-top: 2%;">Acessar</a>
                                    <button type="button" class="btn btn-success" data-bs-toggle="modal" style="margin-top: 2%;"
                                        data-bs-target="#add_conteudo">
                                        Adicionar Conteudo
                                    </button>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
    </section>



    <!-- ===== IONICONS ===== -->
    <script src="https://unpkg.com/ionicons@5.1.2/dist/ionicons.js"></script>

    <!-- ===== MAIN JS ===== -->
    <script src="assets/js/main.js"></script>

    <!-- ===== BOOTSTRAP ===== -->
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.bundle.min.js"
        integrity="sha384-C6RzsynM9kWDrMNeT87bh95OGNyZPhcTNXj1NW7RuBCsyN/o0jlpcV8Qyq46cDfL"
        crossorigin="anonymous"></script>

</body>

</html>
------------------TIAW_aluno.html-------------------
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap@4.0.0/dist/css/bootstrap.min.css"
        integrity="sha384-Gn5384xqQ1aoWXA+058RXPxPg6fy4IWvTNh0E263XmFcJlSAwiGgFAW/dAiS6JXm" crossorigin="anonymous">

    <!-- ===== CSS ===== -->
    <link rel="stylesheet" href="assets/css/styles.css">
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap@4.0.0/dist/css/bootstrap.min.css">
    <title>Conteúdos da Matéria</title>
    <script src="https://code.jquery.com/jquery-3.6.0.min.js"></script>
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@4.0.0/dist/js/bootstrap.min.js"></script>
    <style>
        .card-body iframe {
            display: block;
            margin: 0 auto;
            width: 95%;
            /* Ajuste a largura conforme necessário */
        }
    </style>

    </style>
</head>

<body id="body-pd">
    <a href="painel_aluno.html" class="btn btn-primary">Voltar</a>
    <div class="l-navbar" id="navbar">
        <nav class="nav">
            <div>
                <div class="nav__brand">
                    <ion-icon name="menu-outline" class="nav__toggle" id="nav-toggle"></ion-icon>
                    <a href="painel_aluno.html" class="nav__logo"><img id="logo" src="assets/img/logo.png"
                            width="15%"></a>
                </div>

                <div class="nav__list">
                    <a href="painel_aluno.html" class="nav__link active">
                        <ion-icon name="home-outline" class="nav__icon"></ion-icon>
                        <span class="nav__name">Painel de Controle</span>
                    </a>

                    <a href="mensagem.html" class="nav__link">
                        <ion-icon name="chatbubbles-outline" class="nav__icon"></ion-icon>
                        <span class="nav__name">Mensagem</span>
                    </a>

                    <a href="agenda.html" class="nav__link">
                        <ion-icon name="calendar-outline" class="nav__icon"></ion-icon>
                        <span class="nav__name">Calendario</span>
                    </a>

                    <a href="https://teams.microsoft.com/dl/launcher/launcher.html?url=teams&type=meetup-join&enableMobilePage=true&suppressPrompt=true&tenantId=14cbd5a7-ec94-46ba-b314-cc0fc972a161"
                        class="nav__link">
                        <ion-icon name="tv" class="nav__icon"></ion-icon>
                        <span class="nav__name">Teams</span>
                    </a>


                    <a href="ajuda.html" class="nav__link">
                        <ion-icon name="help-outline" class="nav__icon"></ion-icon>
                        <span class="nav__name">Ajuda</span>
                    </a>

                    <a href="config.html" class="nav__link">
                        <ion-icon name="settings-outline" class="nav__icon"></ion-icon>
                        <span class="nav__name">Configurações</span>
                    </a>
                </div>
            </div>


            <div>
                <img id="foto" src="assets/img/foto.png" width="12%">
            </div>

            <a href="login.html" class="nav__link">
                <ion-icon name="log-out-outline" class="nav__icon"></ion-icon>
                <span class="nav__name">Sair</span>
            </a>
        </nav>
    </div>

    <section class="container-fluid">
        <div class="titulo">
            <h1>
                <h1>Conteúdos da Matéria - Trabalho Interdisciplinar de aplicação web </h1>
            </h1>
        </div>

        <!-- Conteúdo 1 -->
        <div class="card">
            <div class="card-header" id="contentHeading1">
                <h2 class="mb-0">
                    <button class="btn btn-link" type="button" data-toggle="collapse" data-target="#contentCollapse1"
                        aria-expanded="true" aria-controls="contentCollapse1">
                        1 - Apresentação da Disciplina <ion-icon name="arrow-forward-outline"></ion-icon>
                    </button>
                </h2>
            </div>
            <div id="contentCollapse1" class="collapse" aria-labelledby="contentHeading1"
                data-parent="#contentAccordion">
                <div class="card-body">


                    <h3>Explorando o Trabalho Interdisciplinar - Aplicações Web: Uma Visão Simplificada</h3>

                    <p>Sejam bem-vindos à disciplina de Trabalho Interdisciplinar - Aplicações Web! 😄</p>

                    <p>Nesta disciplina, nosso objetivo é guiar vocês pelo processo iterativo e incremental de
                        desenvolvimento de uma aplicação completa, fazendo uso de técnicas e ferramentas de
                        desenvolvimento front-end para a web. Tudo isso acontece por meio do trabalho em equipe.</p>

                    <p>Essa disciplina integra conceitos de outras disciplinas deste semestre, notadamente Algoritmos e
                        Estruturas de Dados, Introdução à Computação e Desenvolvimento de Interfaces Web.</p>

                    <p>A abordagem metodológica adotada nessa disciplina abrange dois frameworks amplamente utilizados
                        na indústria de desenvolvimento de software: o Design Thinking e o Scrum Framework, conforme
                        ilustrado na Figura 1. O Design Thinking é aplicado na primeira etapa, que chamamos de
                        Concepção, onde equipes são formadas e problemas a serem tratados são definidos. Já o Scrum
                        Framework é empregado na segunda etapa, denominada Desenvolvimento.</p>

                    <p>Fonte:
                        <a href="https://jointecnologia.com.br/concepcao-e-desenvolvimento-de-software-com-design-thinking-e-scrum/"
                            target="_blank" rel="noopener noreferrer"> Clique aqui </a>
                    </p>

                    <p>Na primeira etapa, o produto principal é o Backlog do Produto (Product Backlog), que estabelece
                        de forma geral o que será desenvolvido na segunda etapa. Embora haja uma sequência de
                        atividades, existe certa flexibilidade no processo.</p>

                    <p>A condução da disciplina será realizada pelos professores, que acompanharão os alunos desde o
                        início até o fim. É importante destacar que as equipes têm autonomia sobre o rumo do projeto e
                        podem revisar o que está sendo feito a qualquer momento, levando em consideração as lições
                        aprendidas ao longo do processo.</p>

                    <h4>Etapa de Concepção</h4>

                    <p>A primeira parte tem como objetivo definir um problema a ser abordado pelos alunos durante o
                        semestre e formar grupos. Essa etapa segue as etapas de um workshop orientado pelas práticas de
                        Design Thinking. Ao final desta etapa, teremos equipes formadas, um problema definido e uma
                        visão geral da solução a ser implementada, o que chamamos de Product Backlog ou visão de um
                        Produto Mínimo Viável (MVP).</p>

                    <p><strong>Tarefas a serem realizadas:</strong></p>
                    Desenvolvimento das Funcionalidades <br>
                    Definição das estruturas de dados <br>
                    Programação do software (JavaScript) <br>
                    Definição de identidade visual <br>
                    Evolução do relatório técnico do projeto (iniciado na fase de concepção) <br>
                    Elaboração da apresentação do projeto (PowerPoint) <br>
                    Montagem do vídeo do projeto <br>
                    Apresentação do projeto para a turma <br>


                    <p>
                    <h6> Ao final da etapa de Desenvolvimento, espera-se que o grupo entregue uma aplicação totalmente
                        funcional, disponível na Internet, uma apresentação e um vídeo sobre o projeto bem como um
                        relatório técnico com a documentação completa do projeto. </h6>
                    </p>


                </div>
            </div>
        </div>

        <!-- Conteudo 2 -->
        <div class="card">
            <div class="card-header" id="contentHeading2">
                <h2 class="mb-0">
                    <button class="btn btn-link" type="button" data-toggle="collapse" data-target="#contentCollapse2"
                        aria-expanded="true" aria-controls="contentCollapse3">
                        2- Processo de Avaliação<ion-icon name="arrow-forward-outline"></ion-icon>
                    </button>
                </h2>
            </div>
            <div id="contentCollapse2" class="collapse" aria-labelledby="contentHeading2"
                data-parent="#contentAccordion">
                <div class="card-body">


                    <!DOCTYPE html>
                    <html>

                    <head>
                        <title>Processo de Avaliação da Disciplina</title>
                    </head>

                    <body>
                        <h3>Processo de Avaliação</h3>

                        <p>O processo de avaliação está baseado na evolução do software a ser construído pela equipe e
                            mescla avaliações em grupo e avaliações individuais. As entregas são organizadas em 4
                            sprints durante o semestre.</p>

                        <p>É importante ressaltar que não há provas nessa disciplina e não há reavaliação ou outras
                            oportunidades de recuperação.</p>

                        <p>As etapas do processo de avaliação (sprints) e os detalhes de cada etapa são apresentados na
                            figura que se segue e detalhados na sequência.</p>

                        <table border="1">
                            <tr>
                                <th>Atividade</th>
                                <th>Valor</th>
                            </tr>
                            <tr>
                                <td>Avaliação do Desempenho Acadêmico</td>
                                <td>05 pontos</td>
                            </tr>
                            <tr>
                                <td>Sprint 1</td>
                                <td>15 pontos</td>
                            </tr>
                            <tr>
                                <td>Sprint 2</td>
                                <td>20 pontos</td>
                            </tr>
                            <tr>
                                <td>Sprint 3</td>
                                <td>20 pontos</td>
                            </tr>
                            <tr>
                                <td>Sprint 4</td>
                                <td>40 pontos</td>
                            </tr>
                            <tr>
                                <td>Total</td>
                                <td>100 pontos</td>
                            </tr>
                        </table>

                        <h1> Sprint 1 - Concepção do Projeto </h1>
                        <p>Nessa sprint, o trabalho é feito em grupo e a avaliação é realizada pelo professor. A entrega
                            dos artefatos pode ser feita por qualquer membro do grupo a partir das tarefas cadastradas
                            no Canvas.

                            Após a entrega, os membros do grupo apresentam o projeto para toda a turma. A apresentação é
                            obrigatória e pode ser feita por um ou mais membros, a critério do próprio grupo. O aluno ou
                            equipe ausente implicará na perda de 50% dos pontos da sprint 1.

                            O grupo deve entregar e apresentar os artefatos da etapa de concepção que são detalhados na
                            tabela a seguir. </p>


                        <h1> Sprints 2 e 3 - Programação de Funcionalidades </h1>
                        <p>Após a etapa de concepção, é hora de desenvolver o software projetado. O grupo deve se reunir
                            e definir quais serão as funcionalidades que cada membro do grupo ficará responsável. Embora
                            estejam realizando entregas individuais, o grupo deve continuar se reunindo e o trabalho de
                            cada membro deve contribuir para o projeto idealizado durante a concepção. É importante ter
                            em mente que, ao final, na Sprint 4, o grupo deve reunir as contribuições individuais e
                            consolidar em uma entrega única.

                            Assim sendo, nas sprints 2 e 3, cada aluno deve entregar uma implementação que envolve a
                            programação do software e a avaliação é individual. Os detalhes destas entregas constam no
                            menu Tarefas. Para essas entregas, não há apresentação do resultado para toda a turma,
                            apenas para o professor. </p>


                        <h1> Sprint 4 - Projeto Completo </h1>
                        <p>Nessa sprint, o trabalho é feito em grupo novamente e a avaliação é realizada pelo professor.
                            A entrega dos artefatos pode ser feita por qualquer membro do grupo a partir da atividade
                            cadastrada no Canvas. O grupo inteiro é avaliado quanto a forma de organização dos artefatos
                            do projeto, a documentação, a apresentação e o sistema entregue.

                            Após a entrega, os membros do grupo fazem uma apresentação do projeto para toda a turma. A
                            apresentação é obrigatória e pode ser feita por um ou mais membros, a critério do próprio
                            grupo. O aluno ou equipe ausente implicará na perda de 50% dos pontos da sprint 4. </p>



                </div>
            </div>
        </div>



    </section>

    <script src="https://unpkg.com/ionicons@5.1.2/dist/ionicons.js"></script>
    <script src="assets/js/main.js"></script>
    <script src="assets/js/materias.js"></script>


    <!-- ===== IONICONS ===== -->
    <script src="https://unpkg.com/ionicons@5.1.2/dist/ionicons.js"></script>

    <!-- ===== MAIN JS ===== -->
    <script src="assets/js/main.js"></script>

    <!-- ===== BOOTSTRAP ===== -->
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@4.0.0/dist/js/bootstrap.min.js"
        integrity="sha384-JZR6Spejh4U02d8jOt6vLEHfe/JQGiRRSQQxSfFWpi1MquVdAyjUar5+76PVCmYl" crossorigin="anonymous">
        </script>

</body>

</html>
------------------TIAW_Monitor.html-------------------
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap@4.0.0/dist/css/bootstrap.min.css"
        integrity="sha384-Gn5384xqQ1aoWXA+058RXPxPg6fy4IWvTNh0E263XmFcJlSAwiGgFAW/dAiS6JXm" crossorigin="anonymous">

    <!-- ===== CSS ===== -->
    <link rel="stylesheet" href="assets/css/styles.css">
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap@4.0.0/dist/css/bootstrap.min.css">
    <title>Conteúdos da Matéria</title>
    <script src="https://code.jquery.com/jquery-3.6.0.min.js"></script>
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@4.0.0/dist/js/bootstrap.min.js"></script>
    <style>
        .card-body iframe {
            display: block;
            margin: 0 auto;
            width: 95%;
            /* Ajuste a largura conforme necessário */
        }

        .edit-btn,
        .delete-btn {
            position: absolute;
            top: 5px;
            z-index: 999;
            padding: 0.2rem 0.4rem;
            font-size: 0.75rem;
        }

        .edit-btn ion-icon,
        .delete-btn ion-icon {
            font-size: 1rem;
        }

        .edit-btn {
            right: 40px;
            /* Distância da borda direita para o botão de edição */
        }

        .delete-btn {
            right: 5px;
            /* Distância da borda direita para o botão de exclusão */
        }

        .card-header {
            position: relative;
        }
    </style>

    </style>
</head>

<body id="body-pd">
    <a href="painel_monitor.html" class="btn btn-primary">Voltar</a>
    <div class="l-navbar" id="navbar">
        <nav class="nav">
            <div>
                <div class="nav__brand">
                    <ion-icon name="menu-outline" class="nav__toggle" id="nav-toggle"></ion-icon>
                    <a href="painel_monitor.html" class="nav__logo"><img id="logo" src="assets/img/logo.png"
                            width="15%"></a>
                </div>

                <div class="nav__list">
                    <a href="painel_monitor.html" class="nav__link active">
                        <ion-icon name="home-outline" class="nav__icon"></ion-icon>
                        <span class="nav__name">Painel de Controle</span>
                    </a>


                    <a href="mensagem.html" class="nav__link">
                        <ion-icon name="chatbubbles-outline" class="nav__icon"></ion-icon>
                        <span class="nav__name">Mensagem</span>
                    </a>

                    <a href="agenda.html" class="nav__link">
                        <ion-icon name="calendar-outline" class="nav__icon"></ion-icon>
                        <span class="nav__name">Calendario</span>
                    </a>

                    <a href="https://teams.microsoft.com/dl/launcher/launcher.html?url=teams&type=meetup-join&enableMobilePage=true&suppressPrompt=true&tenantId=14cbd5a7-ec94-46ba-b314-cc0fc972a161"
                        class="nav__link">
                        <ion-icon name="tv" class="nav__icon"></ion-icon>
                        <span class="nav__name">Teams</span>
                    </a>


                    <a href="ajuda.html" class="nav__link">
                        <ion-icon name="help-outline" class="nav__icon"></ion-icon>
                        <span class="nav__name">Ajuda</span>
                    </a>

                    <a href="config.html" class="nav__link">
                        <ion-icon name="settings-outline" class="nav__icon"></ion-icon>
                        <span class="nav__name">Configurações</span>
                    </a>
                </div>
            </div>


            <div>
                <img id="foto" src="assets/img/foto.png" width="15%">
            </div>

            <a href="login.html" class="nav__link">
                <ion-icon name="log-out-outline" class="nav__icon"></ion-icon>
                <span class="nav__name">Sair</span>
            </a>
        </nav>
    </div>

    <section class="container-fluid">
        <div class="titulo">
            <h1>
                <h1>Conteúdos da Matéria - Trabalho Interdisciplinar de aplicação web </h1>
            </h1>
        </div>

        <!-- Conteúdo 1 -->
        <div class="card">
            <div class="card-header position-relative" id="contentHeading1">
                <button class="btn btn-primary edit-btn"><ion-icon name="create-outline"></ion-icon></button>
                <button class="btn btn-danger delete-btn"><ion-icon name="trash-outline"></ion-icon></button>
                <h2 class="mb-0">
                    <button class="btn btn-link" type="button" data-toggle="collapse" data-target="#contentCollapse1"
                        aria-expanded="true" aria-controls="contentCollapse1">
                        1 - Apresentação da Disciplina <ion-icon name="arrow-forward-outline"></ion-icon>
                    </button>
                </h2>
            </div>
            <div id="contentCollapse1" class="collapse" aria-labelledby="contentHeading1"
                data-parent="#contentAccordion">
                <div class="card-body">


                    <h3>Explorando o Trabalho Interdisciplinar - Aplicações Web: Uma Visão Simplificada</h3>

                    <p>Sejam bem-vindos à disciplina de Trabalho Interdisciplinar - Aplicações Web! 😄</p>

                    <p>Nesta disciplina, nosso objetivo é guiar vocês pelo processo iterativo e incremental de
                        desenvolvimento de uma aplicação completa, fazendo uso de técnicas e ferramentas de
                        desenvolvimento front-end para a web. Tudo isso acontece por meio do trabalho em equipe.</p>

                    <p>Essa disciplina integra conceitos de outras disciplinas deste semestre, notadamente Algoritmos e
                        Estruturas de Dados, Introdução à Computação e Desenvolvimento de Interfaces Web.</p>

                    <p>A abordagem metodológica adotada nessa disciplina abrange dois frameworks amplamente utilizados
                        na indústria de desenvolvimento de software: o Design Thinking e o Scrum Framework, conforme
                        ilustrado na Figura 1. O Design Thinking é aplicado na primeira etapa, que chamamos de
                        Concepção, onde equipes são formadas e problemas a serem tratados são definidos. Já o Scrum
                        Framework é empregado na segunda etapa, denominada Desenvolvimento.</p>

                    <p>Fonte:
                        <a href="https://jointecnologia.com.br/concepcao-e-desenvolvimento-de-software-com-design-thinking-e-scrum/"
                            target="_blank" rel="noopener noreferrer"> Clique aqui </a>
                    </p>

                    <p>Na primeira etapa, o produto principal é o Backlog do Produto (Product Backlog), que estabelece
                        de forma geral o que será desenvolvido na segunda etapa. Embora haja uma sequência de
                        atividades, existe certa flexibilidade no processo.</p>

                    <p>A condução da disciplina será realizada pelos professores, que acompanharão os alunos desde o
                        início até o fim. É importante destacar que as equipes têm autonomia sobre o rumo do projeto e
                        podem revisar o que está sendo feito a qualquer momento, levando em consideração as lições
                        aprendidas ao longo do processo.</p>

                    <h4>Etapa de Concepção</h4>

                    <p>A primeira parte tem como objetivo definir um problema a ser abordado pelos alunos durante o
                        semestre e formar grupos. Essa etapa segue as etapas de um workshop orientado pelas práticas de
                        Design Thinking. Ao final desta etapa, teremos equipes formadas, um problema definido e uma
                        visão geral da solução a ser implementada, o que chamamos de Product Backlog ou visão de um
                        Produto Mínimo Viável (MVP).</p>

                    <p><strong>Tarefas a serem realizadas:</strong></p>
                    Desenvolvimento das Funcionalidades <br>
                    Definição das estruturas de dados <br>
                    Programação do software (JavaScript) <br>
                    Definição de identidade visual <br>
                    Evolução do relatório técnico do projeto (iniciado na fase de concepção) <br>
                    Elaboração da apresentação do projeto (PowerPoint) <br>
                    Montagem do vídeo do projeto <br>
                    Apresentação do projeto para a turma <br>


                    <p>
                    <h6> Ao final da etapa de Desenvolvimento, espera-se que o grupo entregue uma aplicação totalmente
                        funcional, disponível na Internet, uma apresentação e um vídeo sobre o projeto bem como um
                        relatório técnico com a documentação completa do projeto. </h6>
                    </p>


                </div>
            </div>
        </div>

        <!-- Conteudo 2 -->
        <div class="card">
            <div class="card-header position-relative" id="contentHeading1">
                <button class="btn btn-primary edit-btn"><ion-icon name="create-outline"></ion-icon></button>
                <button class="btn btn-danger delete-btn"><ion-icon name="trash-outline"></ion-icon></button>
                <h2 class="mb-0">
                    <button class="btn btn-link" type="button" data-toggle="collapse" data-target="#contentCollapse2"
                        aria-expanded="true" aria-controls="contentCollapse3">
                        2- Processo de Avaliação<ion-icon name="arrow-forward-outline"></ion-icon>
                    </button>
                </h2>
            </div>
            <div id="contentCollapse2" class="collapse" aria-labelledby="contentHeading2"
                data-parent="#contentAccordion">
                <div class="card-body">


                    <!DOCTYPE html>
                    <html>

                    <head>
                        <title>Processo de Avaliação da Disciplina</title>
                    </head>

                    <body>
                        <h3>Processo de Avaliação</h3>

                        <p>O processo de avaliação está baseado na evolução do software a ser construído pela equipe e
                            mescla avaliações em grupo e avaliações individuais. As entregas são organizadas em 4
                            sprints durante o semestre.</p>

                        <p>É importante ressaltar que não há provas nessa disciplina e não há reavaliação ou outras
                            oportunidades de recuperação.</p>

                        <p>As etapas do processo de avaliação (sprints) e os detalhes de cada etapa são apresentados na
                            figura que se segue e detalhados na sequência.</p>

                        <table border="1">
                            <tr>
                                <th>Atividade</th>
                                <th>Valor</th>
                            </tr>
                            <tr>
                                <td>Avaliação do Desempenho Acadêmico</td>
                                <td>05 pontos</td>
                            </tr>
                            <tr>
                                <td>Sprint 1</td>
                                <td>15 pontos</td>
                            </tr>
                            <tr>
                                <td>Sprint 2</td>
                                <td>20 pontos</td>
                            </tr>
                            <tr>
                                <td>Sprint 3</td>
                                <td>20 pontos</td>
                            </tr>
                            <tr>
                                <td>Sprint 4</td>
                                <td>40 pontos</td>
                            </tr>
                            <tr>
                                <td>Total</td>
                                <td>100 pontos</td>
                            </tr>
                        </table>

                        <h1> Sprint 1 - Concepção do Projeto </h1>
                        <p>Nessa sprint, o trabalho é feito em grupo e a avaliação é realizada pelo professor. A entrega
                            dos artefatos pode ser feita por qualquer membro do grupo a partir das tarefas cadastradas
                            no Canvas.

                            Após a entrega, os membros do grupo apresentam o projeto para toda a turma. A apresentação é
                            obrigatória e pode ser feita por um ou mais membros, a critério do próprio grupo. O aluno ou
                            equipe ausente implicará na perda de 50% dos pontos da sprint 1.

                            O grupo deve entregar e apresentar os artefatos da etapa de concepção que são detalhados na
                            tabela a seguir. </p>


                        <h1> Sprints 2 e 3 - Programação de Funcionalidades </h1>
                        <p>Após a etapa de concepção, é hora de desenvolver o software projetado. O grupo deve se reunir
                            e definir quais serão as funcionalidades que cada membro do grupo ficará responsável. Embora
                            estejam realizando entregas individuais, o grupo deve continuar se reunindo e o trabalho de
                            cada membro deve contribuir para o projeto idealizado durante a concepção. É importante ter
                            em mente que, ao final, na Sprint 4, o grupo deve reunir as contribuições individuais e
                            consolidar em uma entrega única.

                            Assim sendo, nas sprints 2 e 3, cada aluno deve entregar uma implementação que envolve a
                            programação do software e a avaliação é individual. Os detalhes destas entregas constam no
                            menu Tarefas. Para essas entregas, não há apresentação do resultado para toda a turma,
                            apenas para o professor. </p>


                        <h1> Sprint 4 - Projeto Completo </h1>
                        <p>Nessa sprint, o trabalho é feito em grupo novamente e a avaliação é realizada pelo professor.
                            A entrega dos artefatos pode ser feita por qualquer membro do grupo a partir da atividade
                            cadastrada no Canvas. O grupo inteiro é avaliado quanto a forma de organização dos artefatos
                            do projeto, a documentação, a apresentação e o sistema entregue.

                            Após a entrega, os membros do grupo fazem uma apresentação do projeto para toda a turma. A
                            apresentação é obrigatória e pode ser feita por um ou mais membros, a critério do próprio
                            grupo. O aluno ou equipe ausente implicará na perda de 50% dos pontos da sprint 4. </p>



                </div>
            </div>
        </div>



    </section>

    <script src="https://unpkg.com/ionicons@5.1.2/dist/ionicons.js"></script>
    <script src="assets/js/main.js"></script>
    <script src="assets/js/materias.js"></script>


    <!-- ===== IONICONS ===== -->
    <script src="https://unpkg.com/ionicons@5.1.2/dist/ionicons.js"></script>

    <!-- ===== MAIN JS ===== -->
    <script src="assets/js/main.js"></script>

    <!-- ===== BOOTSTRAP ===== -->
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@4.0.0/dist/js/bootstrap.min.js"
        integrity="sha384-JZR6Spejh4U02d8jOt6vLEHfe/JQGiRRSQQxSfFWpi1MquVdAyjUar5+76PVCmYl" crossorigin="anonymous">
        </script>

</body>

</html>

