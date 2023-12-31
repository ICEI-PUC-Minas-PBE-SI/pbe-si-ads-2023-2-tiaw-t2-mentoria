# Informações do Projeto 

SISTEMA WEB PARA GESTÃO DE MONITORIAS NA PUC MINAS

Faculdades: Sistemas de Informação e Análise e Desenvolvimento de Sistemas

## Participantes

Desenvolvedores: 

Adenilson Rodrigues Cordeiro Junior

Arthur Alves Oliveira Silva

Alessandro Gomes Pereira

Marlon Magalhaes Carvalho

Samuel Correia Nunes


# Estrutura do Documento

- [Informações do Projeto](#informações-do-projeto)
  - [Participantes](#participantes)
- [Estrutura do Documento](#estrutura-do-documento)
- [Introdução](#introdução)
  - [Problema](#problema)
  - [Objetivos](#objetivos)
  - [Justificativa](#justificativa)
  - [Público-Alvo](#público-alvo)
- [Especificações do Projeto](#especificações-do-projeto)
  - [Personas e Mapas de Empatia](#personas-e-mapas-de-empatia)
  - [Histórias de Usuários](#histórias-de-usuários)
  - [Requisitos](#requisitos)
    - [Requisitos Funcionais](#requisitos-funcionais)
    - [Requisitos não Funcionais](#requisitos-não-funcionais)
  - [Restrições](#restrições)
- [Projeto de Interface](#projeto-de-interface)
  - [User Flow](#user-flow)
  - [Wireframes](#wireframes)
- [Metodologia](#metodologia)
  - [Divisão de Papéis](#divisão-de-papéis)
  - [Ferramentas](#ferramentas)
  - [Controle de Versão](#controle-de-versão)
- [**############## SPRINT 1 ACABA AQUI #############**](#-sprint-1-acaba-aqui-)
- [Projeto da Solução](#projeto-da-solução)
  - [Tecnologias Utilizadas](#tecnologias-utilizadas)
  - [Arquitetura da solução](#arquitetura-da-solução)
- [Avaliação da Aplicação](#avaliação-da-aplicação)
  - [Plano de Testes](#plano-de-testes)
  - [Registros de Testes](#registros-de-testes)
- [Referências](#referências)


# Introdução

## Problema
  Para muitos estudantes, a busca por orientação ou monitoria pode ser dificultada por equívocos e desafios significativos. Algumas pessoas encaram essa busca como um sinal de vulnerabilidade ou falta de competência, o que acaba por desencorajá-las a procurar monitores. Além disso, estudantes universitários frequentemente enfrentam uma carga horária intensa, equilibrando aulas e trabalho, o que gera uma sensação de sobrecarga e falta de tempo para se envolver na busca por um monitor. A dificuldade em coordenar agendas também é um obstáculo adicional, especialmente quando os monitores em potencial também estão sobrecarregados com suas próprias obrigações acadêmicas e profissionais.

  Nesse cenário desafiador, a sincronização das agendas dos alunos com as dos monitores torna-se uma tarefa complicada, frequentemente desencorajando a busca por monitoria. No entanto, é importante reconhecer que esses obstáculos não deveriam impedir os estudantes de buscar orientação. Apesar das dificuldades, os benefícios que a monitoria pode oferecer em suas jornadas acadêmicas e profissionais são imensuráveis. Portanto, é fundamental superar esses desafios, procurando ativamente monitores que possam oferecer orientação valiosa.

## Objetivos

Desenvolver um software web voltado para a gestão do processo de aprendizado entre monitores e monitorados, com foco na facilitação da comunicação entre ambas as partes, incluindo a seleção do monitor e a definição dos tópicos a serem abordados durante a monitoria.

Objetivos Específicos:
Este projeto se propõe a alcançar os seguintes objetivos:

- Realizar uma pesquisa preliminar para identificar e definir os desafios associados ao processo de monitoria.
- Conduzir uma análise detalhada da documentação de requisitos, visando a identificação dos elementos cruciais para a criação do software.
- Criar uma aplicação web que permita a marcação e administração de sessões de monitoria por meio de módulos e funcionalidades específicas.
- Utilizar técnicas de desenvolvimento web para a construção da interface e layout da plataforma, garantindo também a implementação das funcionalidades necessárias.

Deste modo, nosso objetivo é desenvolver um software web que facilite eficazmente a gestão do processo de monitoria, promovendo a interação entre monitor e monitorado, ao mesmo tempo em que simplifica a escolha do monitor e a definição dos temas a serem abordados durante as sessões.

## Justificativa

  O software monitoria foi concebido com o propósito fundamental de revolucionar a interação entre os alunos e monitores da PUC Minas, com o objetivo primordial de simplificar e aprimorar substancialmente o canal de comunicação entre esses dois grupos, visando proporcionar uma experiência global aprimorada. Apesar de a plataforma CANVAS já oferecer a funcionalidade de monitoria, o atual modelo não está plenamente alinhado com as necessidades dos usuários que buscam especificamente esse tipo de interação. Nesse contexto, essa questão adquire grande relevância, especialmente para os alunos ingressantes da universidade, que frequentemente não estão familiarizados com o funcionamento detalhado do CANVAS e do SGA, o que resulta em desconhecimento e limitações na sua utilização eficiente.

  A implementação dessas melhorias não apenas beneficiará os alunos, proporcionando-lhes uma experiência mais suave e produtiva, mas também terá impactos positivos significativos para os monitores, contribuindo para a otimização e aprimoramento da eficácia do processo para todas as partes envolvidas permitindo a ambos novas funcionalidades para a melhor condução do processo de monitoria.

## Público-Alvo

O software web de monitorias para instituições educacionais atende a diversos públicos, incluindo:

- Professores e Orientadores: Utilizam a plataforma para fornecer suporte acadêmico e orientação aos estudantes.
- Alunos: Acessam a ferramenta para aprimorar seu desempenho acadêmico e planejar suas sessões de monitoria.
- Coordenadores Educacionais: Responsáveis pela supervisão de diversas atividades, incluindo as monitorias, contam com o software para gerenciar esses processos de forma eficiente.
- Administração Escolar: Os membros da equipe administrativa utilizam a plataforma para garantir o funcionamento adequado de todas as operações relacionadas às monitorias e à gestão geral da instituição.
 
# Especificações do Projeto

## Personas e Mapas de Empatia
**Persona(1);**

![PS_Maria_Gabriela](images/PS_Maria_Gabriela.png)
![ME_Maria_Gabriela](images/ME_Maria_Gabriela.png)

**Persona(2);**

![PS_Mateus_Prado](images/PS_Mateus_Prado.png)
![ME_Mateus_Prado](images/ME_Mateus_Prado.png)

**Persona(3);**

![PS_Rafaela_Santos](images/PS_Rafaela_Santos.png)
![ME_Rafaela_Santos](images/ME_Rafaela_Santos.png)


## Histórias de Usuários
--------------------------------------------------------------------------------------------------------------------
Maria Gabriela Amorim é estudante do curso de Psicologia na PUC Minas e leva uma vida extremamente ocupada. Ela enfrenta desafios consideráveis na tentativa de equilibrar seus horários de estudo com seus compromissos pessoais e profissionais. Durante nossa entrevista, ela destacou a dificuldade que enfrenta ao buscar suporte para as disciplinas em que encontra obstáculos. Isso ocorre, em grande parte, devido à maioria das sessões de monitoria ocorrerem durante as tardes e, frequentemente, de forma presencial. No entanto, devido à sua residência distante e ao seu estágio em uma grande empresa, Gabriela não tem a flexibilidade de comparecer a essas monitorias.
Ela está ansiosa por uma solução que lhe permita harmonizar sua agenda com a disponibilidade das monitorias de forma híbrida, o que significa que ela gostaria de poder escolher entre participar presencialmente em alguns dias e remotamente em outros, conforme sua situação e necessidades específicas.

--------------------------------------------------------------------------------------------------------------------
Mateus Júnior Prado é um estudante dedicado do curso de Sistemas de Informação na PUC Minas. Desde o início de sua jornada acadêmica, ele traçou com clareza seus objetivos: tornar-se um programador habilidoso e, eventualmente, alcançar o sucesso como desenvolvedor de software. No entanto, Mateus compreendia que a estrada para atingir esses objetivos seria longa e repleta de desafios. Um dos obstáculos que ele enfrentou desde o início de sua trajetória foi a necessidade de orientação e monitoria.
Ele reconhecia a importância de aprender com aqueles que já trilharam o caminho que ele desejava seguir, mas deparava-se com a constante dificuldade de encontrar monitores e agendar sessões de monitoria que se encaixassem em sua agenda lotada de aulas e projetos. Determinado a superar esse obstáculo, Mateus começou a buscar métodos ágeis e flexíveis para programar e realizar suas monitorias. Ele percebeu que o mundo digital oferece uma infinidade de soluções e estava decidido a aproveitar ao máximo esses recursos.

--------------------------------------------------------------------------------------------------------------------
Rafaela Alves Santos é estudante do curso de Farmácia na PUC Minas. Ela tem a necessidade de entrar em contato com a monitoria da universidade de maneira ágil e eficiente. Seu objetivo é escolher as disciplinas que requerem sua maior atenção. Essa busca por agilidade e facilidade no acesso ao sistema de monitoria tem como finalidade principal auxiliá-la nos estudos das matérias em que enfrenta maiores dificuldades. Ela tem o desejo em economizar tempo e melhorar seu desempenho acadêmico, aproveitando da oportunidade para esclarecer dúvidas com os monitores, tornando seu processo de aprendizado mais eficaz.

--------------------------------------------------------------------------------------------------------------------

Com base nas análises das personas e nos mapas de empatia, foram identificados os seguintes pontos a serem desenvolvidos:

|MARIA GABRIELA      | QUERO/PRECISO                            |PARA                                                  |
|--------------------|------------------------------------------|------------------------------------------------------|
|Usuário do sistema  | Agendar as monitorias                     | Conciliar as agendas                                 |
|Usuário do sistema  | monitorias na modalidade Remota/Presencial| Flexibilidade de atendimento                         |

|MATEUS JUNIOR       | QUERO/PRECISO                            |PARA                                                  |
|--------------------|------------------------------------------|------------------------------------------------------|
|Usuário do sistema  | Agendar as monitorias                     | Conciliar as agendas                                 |
|Usuário do sistema  | monitorias na modalidade Remota/Presencial| Flexibilidade de atendimento                         |
|Usuário do sistema  | Sistema de Feedback                      | Criticas em relação as disponibilidades dos monitores |


|RAFAELA ALVES       | QUERO/PRECISO                            |PARA                                                  |
|--------------------|------------------------------------------|------------------------------------------------------|
|Usuário do sistema  | Agendar as monitorias                     | Conciliar as agendas                                 |
|Usuário do sistema  | Comunicar com o monitor                   | Sanar duvidas                                        |
|Usuário do sistema  | monitorias na modalidade Remota/Presencial| Flexibilidade de atendimento                         |
|Usuário do sistema  | Sistema de Feedback                      | Criticas em relação as disponibilidades dos monitores |
|Usuário do sistema  | Suporte ao Sistema                       | Auxiliar na utilização do novo sistema               |




## Requisitos

As tabelas subsequentes exibem os requisitos funcionais e não funcionais que proporcionam uma descrição detalhada do escopo do projeto.

### Requisitos Funcionais

|ID    | Descrição do Requisito  | Prioridade |
|------|-----------------------------------------|----|
|RF-001| O sistema deve ter um banco de dados de alunos e monitores | ALTA |
|RF-002| Permitir o cadastro das disciplinas  | ALTA |
|RF-003| Disponibilizar agenda para marcação de horários com monitores | ALTA |
|RF-004| Sistema de Mensagem para comunicação entre monitor e Aluno | ALTA |
|RF-005| O sistema deve permitir a entrada por Login e Senha | ALTA |
|RF-006| Compartilhamento de Recursos e Matérias Complementares | MÉDIO |
|RF-007| O sistema deve possuir encaminhamento para sites que possibilitem o Feedback dos alunos| BAIXO |


### Requisitos não Funcionais

|ID     | Descrição do Requisito  |Prioridade |
|-------|-------------------------|----|
|RNF-001| O sistema deve ser capaz de ser escalavel | ALTA | 
|RNF-002| O sistema deve possuir medidas de segurança visando a privacidade dos dados  | ALTA | 
|RNF-003| O sistema deve ser robusto o suficiente para suportar simultaneamente múltiplos usuários.| ALTA | 
|RNF-004| O sistema deve ser responsivo para rodar em um dispositivos móvel  | MÉDIA | 
|RNF-005| O sistema deve possuir Backup planejado dos dados  | MÉDIA | 
|RNF-006| O sistema deve possuir suporte tecnico quando necessario | MÉDIA | 
|RNF-007| O sistema deve estar disponível 99,9% do tempo, sem interrupções, excluindo janelas de manutenção planejada. | BAIXO | 


## Restrições

O projeto está limitado pelos elementos apresentados na tabela a seguir.

|ID| Restrição                                             |
|--|-------------------------------------------------------|
|01| O sistema web será desenvolvido visando apenas desktops.|
|02| O projeto deverá ser concluído até o final do semestre letivo.|
|03| O projeto possui 5 desenvolvedores.|
|04| Restrições orçamentárias e financeiras.|
|05| O sistema deverá ser desenvolvido em JavaScript.|
|06| O sistema deve ser desenvolvido em língua portuguesa.|



# Projeto de Interface

Estas soluções foram minuciosamente planejadas com o objetivo de proporcionar uma experiência completa e eficaz aos usuários. Um elemento essencial do nosso site será a incorporação de um sistema de mensagem que permitirá a interação direta entre os usuários e os monitores. Isso simplificará a troca eficaz de informações e experiências, possibilitando que os usuários esclareçam dúvidas, recebam orientações e estabeleçam conexões mais próximas com os monitores, enriquecendo assim o processo de monitoria.

Ademais, o site incluirá uma funcionalidade de agendamento que permitirá aos monitores marcar sessões de monitoria de acordo com sua disponibilidade. Essa funcionalidade aprimorará a gestão do tempo, assegurando uma organização eficiente das agendas e proporcionando transparência na disponibilidade dos monitores.

Um recurso valioso será a integração de um fórum no site, onde os usuários poderão compartilhar suas experiências, fazer perguntas e colaborar uns com os outros. Esse espaço comunitário promoverá a colaboração e a troca de conhecimento entre os usuários, enriquecendo ainda mais a experiência educacional.

Por fim, nosso site incluirá uma aba dedicada à inclusão de listas de atividades, vídeos e materiais complementares disponibilizados pelos monitores. Além disso, o site também contará com uma página dedicada ao feedback. Isso permitirá que os usuários realizem tarefas e avaliem tanto os monitores quanto o conteúdo disponibilizado. Essa abordagem não apenas incentivará a participação ativa, mas também possibilitará o aprimoramento contínuo do programa de monitoria com base nos comentários dos usuários.


## User Flow

![User_Flow](images/User_Flow.png)


## Wireframes
**Wireframe: Login**

![Login](images/Tela_Login.png)

**Wireframe: Painel do Aluno**

![Painel Aluno](images/Tela_Painel_Aluno.png)

**Wireframe: Painel do Monitor**

![Painel Monitor](images/Tela_Painel_Monitor.png)

**Wireframe: Conteúdo das Disciplinas**

![Disciplinas](images/Tela_Cont.Disciplinas.png)

**Wireframe: Agendamento**

![Calendario](images/Tela_Calendario.png)

**Wireframe: Mensagens**

![Mensagens](images/Tela_Mensagens.png)

**Wireframe: Ajuda**

![Ajuda](images/Tela_Ajuda.png)

**Wireframe: Configurações**

![Configuracao](images/Tela_Configuração.png)


# Metodologia


A metodologia adotada pelo nosso grupo para o desenvolvimento deste projeto baseou-se nas práticas ágeis, uma abordagem que valoriza a flexibilidade, a colaboração e a entrega contínua. Optamos por utilizar o Scrum, um dos métodos ágeis mais reconhecidos, para guiar nosso processo de trabalho. 
A metodologia enfatiza a entrega incremental, permitindo que as funcionalidades do projeto sejam desenvolvidas e disponibilizadas em ciclos curtos, conhecidos como sprints. Cada sprint teve uma duração fixa, proporcionando oportunidades frequentes de revisão e adaptação do trabalho realizado. 
Para facilitar a comunicação e colaboração, utilizamos ferramentas colaborativas, como o discord para comunicação em tempo real e o Trello para gerenciar as tarefas em um formato visual e interativo. Essas ferramentas foram essenciais para manter todos os membros da equipe alinhados com os objetivos e progressos do projeto. 

## Divisão de Papéis

A equipe foi dividida em papéis distintos, cada membro contribuindo para o desenvolvimento do projeto de maneira específica. Abaixo estão detalhadas as responsabilidades e realizações de cada integrante:

Adenilson:
Alinhou os cards do Painel de Controle.
Uniformizou o tamanho das imagens da capa do álbum.
Reduziu e otimizou os nomes das páginas do projeto.
Aprimorou a estilização da Página de Conteúdo com ícones e fontes.
Desenvolveu um Novo Painel do Monitor no Estilo de Postagem de Blog.
Criou botões exclusivos para o Monitor/Professor, permitindo apagar o conteúdo postado semanalmente e editar.

Alessandro:
Adicionou os novos inputs da Página Calendário ao Calendário.
Desenvolveu um botão para o envio de imagens da capa dos cards/configuração.
Incluiu botões de alternância Light/Dark na agenda.
Integrado o calendário dentro de um container Bootstrap para garantir responsividade.
Realizou a limpeza do código da página desenvolvida.

Arthur:
Verificou a responsividade da tela desenvolvida.
Corrigiu o botão "Voltar" na Página dos Conteúdos das Disciplinas.
Garantiu que todas as páginas estão linkadas corretamente.
Melhorou e corrigiu o conteúdo das páginas, removendo informações desnecessárias.
Corrigiu nomes e e-mails na página de pessoas.
Adicionou um link na página de ajuda para os contatos da PUC.

Marlon:
Vinculou no código a imagem "Fale com a PUC Minas" com o site oficial da PUC Minas.
Desenvolveu páginas de Caixa de Saída, Importantes e Lixeira.
Garantiu a correta vinculação de todas as páginas.
Realizou uma revisão geral do trabalho, verificando responsividade, conexões, links, comunicação e GitHub.
Supervisionou a equipe para as entregas dentro do prazo estabelecido.

Samuel:
Desenvolveu o botão "Sair" para todas as páginas.
Inseriu ícones na página de ajuda para cada opção.
Verificou a responsividade do Menu Lateral das páginas.
Realizou a limpeza do código em todas as páginas.
Desenvolveu a página do monitor, incluindo a barra lateral.
Coordenou a equipe em direção às metas e sprints.
Foi responsável por corrigir erros, códigos, documentos e assegurou a qualidade do trabalho em cada sprint.

## Ferramentas

No processo de desenvolvimento de um software web voltado para a gestão de processo de aprendizado entre monitores e monitorados, diversas ferramentas desempenharam papéis cruciais. Cada uma delas contribuiu para diferentes aspectos do ciclo de vida do software, desde o planejamento até a entrega final. Abaixo, destacamos as principais ferramentas utilizadas e suas respectivas usabilidades e vantagens:

Trello - Controle de Demandas e Gerenciamento de Projeto:

O Trello é uma ferramenta de gerenciamento de projetos baseada em quadros, listas e cartões. Cada cartão representa uma tarefa ou demanda, e as listas organizam essas tarefas em diferentes estágios do projeto, isso facilita a visualização do fluxo de trabalho, permite atribuir responsabilidades a membros da equipe, acompanhar o progresso em tempo real e identificar possíveis gargalos. Além disso, sua interface intuitiva promove a colaboração eficiente entre os membros da equipe.

VSCode - Desenvolvimento de HTML5, CSS e JS (JavaScript):

Visual Studio Code (VSCode) é um ambiente de des’envolvimento integrado leve e poderoso. Suporta uma ampla gama de linguagens de programação, oferecendo recursos avançados como realce de sintaxe, depuração e controle de versão integrado. A eficiência do VSCode reside na sua extensibilidade e na integração perfeita com ferramentas populares. Oferece sugestões inteligentes de código, facilita a navegação no projeto e proporciona uma experiência de desenvolvimento fluida.

Discord - Reuniões de Alinhamento:

Discord é uma plataforma de comunicação por voz, vídeo e texto. Foi utilizado para reuniões de alinhamento entre os membros da equipe, proporcionando uma comunicação rápida e eficaz. Foram realizadas reuniões síncronas, promovendo a interação instantânea entre os membros da equipe, facilita a comunicação informal e oferece recursos como compartilhamento de tela para apresentações mais claras.

GitHub - Controle de versão do software e repositório de documentação:

GitHub é uma plataforma de hospedagem de código-fonte que utiliza o sistema de controle de versão Git. Ele fornece um ambiente colaborativo para desenvolvedores compartilharem, colaborarem e controlarem as alterações em seu código. O repositório oferece um histórico detalhado de alterações no código, facilita a colaboração simultânea de várias equipes, fornece recursos de rastreamento de problemas (issues) e permite a integração contínua para garantir uma entrega contínua e estável.
Em conjunto, essas ferramentas criaram um ambiente de desenvolvimento integrado e colaborativo. O Trello ajudou na organização das tarefas, o VSCode facilitou o desenvolvimento do código, o Discord promoveu a comunicação eficiente, e o GitHub garantiu o controle de versão e a gestão centralizada do código-fonte.


| Ambiente  | Plataforma              |Link de Acesso |
|-----------|-------------------------|---------------|
|Gerenciamento de projeto  | Trello |  https://trello.com/ | 
|Repositório de código | GitHub | https://gist.github.com/ | 
|Ambiente de desenvolvimento | VScode |  https://code.visualstudio.com/ | 
|Reuniões de alinhamento | Discord | https://discord.com/ | 

## Controle de Versão

O controle de versão é uma parte essencial do desenvolvimento de software, e o GitHub emergiu como uma plataforma central nesse processo, oferecendo inúmeras vantagens para desenvolvedores individuais e equipes. Sua importância transcende a simples hospedagem de código, desempenhando um papel fundamental em promover a colaboração, garantir a integridade do código e facilitar o desenvolvimento iterativo. As seguintes funcionalidades foram utilizadas no processo de desenvolvimento do projeto:

  1.	Branches:
•	Master: A branch "master" é utilizada para armazenar versões estáveis e testadas do software. É a versão que está pronta para produção.
•	Unstable: A branch "unstable" contém versões testadas, mas que ainda podem apresentar instabilidades. É uma etapa intermediária antes da versão estável.
•	Testing: A branch "testing" é destinada a versões em processo de teste. Aqui, as funcionalidades são agrupadas para verificar sua estabilidade antes de passar para a branch "unstable" ou "master".
•	Dev: A branch "dev" é a versão de desenvolvimento, onde as novas funcionalidades são integradas e testadas continuamente.
  2.	Commits:
•	Cada commit no repositório representa uma alteração específica no código.
•	Commits são feitos de forma atômica, abordando uma única funcionalidade ou correção por vez.
•	Mensagens de commit são claras e informativas, seguindo as melhores práticas de commit messages.
  3.	Merges:
•	Merges são realizados conforme as funcionalidades são desenvolvidas e testadas com sucesso na branch "dev".
•	Integrações de branches ocorrem regularmente para evitar conflitos e manter um fluxo contínuo de desenvolvimento.
•	Merges para branches de teste e instável são realizados apenas após testes completos e aprovação.
  4.	Tags:
•	Tags são usadas para marcar versões específicas do software, especialmente aquelas que são lançadas para produção.
•	Cada tag é nomeada de acordo com a versão correspondente para fácil referência.

Gerência de Issues: Convenção de Etiquetas
  1.	Bugfix:
•	Issues rotuladas como "bugfix" indicam problemas em funcionalidades existentes que precisam ser corrigidos.
•	A equipe prioriza e aborda esses problemas de forma eficiente, realizando os devidos testes antes de fazer os merges.
  2.	Enhancement:
•	Issues rotuladas como "enhancement" indicam áreas de funcionalidades existentes que precisam ser aprimoradas.
•	As melhorias propostas são discutidas e implementadas na branch de desenvolvimento, passando por testes adequados.
  3.	Feature:
•	Issues rotuladas como "feature" representam a introdução de novas funcionalidades.
•	As novas funcionalidades são desenvolvidas na branch de desenvolvimento ("dev") e integradas de acordo com o fluxo estabelecido.

Essa estrutura e convenção de nomenclatura proporcionam uma organização clara e eficiente no desenvolvimento do software, permitindo uma gestão robusta e controlada do ciclo de vida do projeto, desde o desenvolvimento até a entrega estável em produção. O GitHub, como plataforma de hospedagem, facilita a colaboração entre membros da equipe, o rastreamento de mudanças e o gerenciamento de problemas, tornando o processo mais transparente e eficaz.

# Projeto da Solução

## Tecnologias Utilizadas

No decorrer do desenvolvimento deste projeto, tornou-se imprescindível a criação de códigos HTML (Hypertext Markup Language), cuja finalidade é possibilitar que o navegador interprete e exiba as marcações de texto e outros elementos de mídia em uma página web. Essa abordagem visa viabilizar uma interação eficaz do usuário com o conteúdo disponibilizado.

O papel crucial desempenhado pelo desenvolvimento do código CSS (Cascading Style Sheets) concentrou-se na estilização do site, resultando em uma interface de navegação mais atraente e amigável ao usuário. Isso elevou significativamente a experiência de utilização para um nível mais sofisticado e agradável.

Vale ressaltar que foi necessário empregar o framework front-end Bootstrap, que oferece estruturas de CSS para a criação de sites e aplicações responsivas de maneira ágil e simplificada. Este framework contribuiu de maneira significativa para a eficiência e a estética do projeto.

No âmbito deste trabalho, a linguagem de programação JavaScript desempenhou um papel fundamental. Ela permitiu a criação de funções dinâmicas que aprimoraram a experiência do usuário durante a interação com o site. Além disso, por meio do JavaScript, foi possível manipular objetos e elementos, viabilizando o funcionamento de partes específicas do programa. Essa versatilidade e capacidade de interação dinâmica foram elementos-chave na implementação bem-sucedida do projeto.

O jQuery desempenhou um papel essencial no desenvolvimento da página web, proporcionando uma série de funções que auxiliam os programadores a escrever de maneira mais rápida e dinâmica o DOM (Document Object Model), sem a necessidade de criar o código completo em JavaScript. Essa ferramenta simplifica tarefas comuns, oferecendo uma abstração eficaz sobre as complexidades do JavaScript puro, o que resulta em um desenvolvimento mais eficiente e produtivo. Ao utilizar o jQuery, foi possível otimizar o processo de manipulação e interação com os elementos da página, contribuindo para uma experiência de usuário mais fluida e agradável.

Para aprimorar a estilização do site, optou-se por incorporar a biblioteca de ícones do FontAwesome. Essa escolha permitiu enriquecer visualmente o design, proporcionando uma ampla variedade de ícones que foram facilmente integrados às diferentes partes do site. A utilização da biblioteca FontAwesome não apenas aprimorou a estética geral, mas também contribuiu para uma experiência de usuário mais intuitiva e visualmente atraente, enriquecendo a representação gráfica dos elementos presentes na página.

A seguir, apresentamos as primeiras versões iniciais do sistema:

Este constitui o primeiro esboço da tela do painel do usuário, onde inicialmente concebemos a ideia de integrar todas as funcionalidades do site em uma única tela. Entretanto, essa abordagem logo se mostrou inviável devido à complexidade do projeto.

![Wireframe](images/Wireframe.png)

A partir do esboço mencionado anteriormente, evoluímos para esta interface, utilizando exclusivamente recursos de HTML, CSS e Bootstrap. No entanto, à medida que o projeto avançava, tornou-se evidente a necessidade de aprimorar a interface desenvolvida, buscando um design mais moderno e atualizado.

![Wireframe1](images/Wireframe_1.jpeg)

Finalmente, apresentamos a versão definitiva do projeto, na qual os conceitos foram meticulosamente revisados e refinados. Nessa interface, adotamos uma abordagem mais sóbria e contemporânea. Adicionalmente, em consonância com a visão inicial delineada no primeiro esboço, buscamos a padronização das funcionalidades em um único layout, assegurando a uniformidade do conteúdo em diversas telas. Este processo de aprimoramento teve como objetivo não apenas aprimorar a estética, mas também promover a consistência e a usabilidade em todas as áreas do site.

![Wireframe2](images/Wireframe_2.png)


**Esboço Escrito: Detalhamento das Funcionalidades e Ferramentas no Contexto Acadêmico**

1. *Página do Aluno:*
   - *Wireframes:* Desenvolvimento de esboços para a página inicial, visualização de disciplinas, mensagens e detalhes da disciplina.
   - *Interação:* Utilização de HTML, CSS e Bootstrap para criar páginas responsivas e amigáveis. Além disso, o uso dessas tecnologias para implementar interatividade, como navegação entre disciplinas, visualização de vídeos, textos e envio de mensagens.

2. *Página do Monitor:*
   - *Wireframes:* Desenvolvimento de wireframes para a adição de novas disciplinas, upload de conteúdo e interação com alunos.
   - *Interação:* Utilização de HTML, CSS, Bootstrap e JavaScript para criar uma interface intuitiva, permitindo ao monitor adicionar disciplinas, conteúdos e interagir com os alunos.

3. *Caixa de Mensagens:*
   - *Wireframes:* Prototipagem da interface de mensagens, incluindo envio, recebimento e listagem de mensagens.
   - *Interação:* Uso de JavaScript para implementar funcionalidades de mensagens, tornando a comunicação entre alunos e monitores eficiente.

4. *Agenda:*
   - *Wireframes:* Esboço da estrutura da agenda, exibição de datas importantes, prazos de entrega, etc.
   - *Interação:* Implementação da lógica para exibir e gerenciar datas importantes usando JavaScript. Isso permitirá que alunos e monitores acompanhem eventos cruciais no contexto acadêmico.

5. *Tela de Login:*
   - *Wireframes:* Criação de wireframes para a página de login, destacando campos de usuário e senha.
   - *Interação:* Desenvolvimento de autenticação com Node.js e Express, garantindo a segurança ao armazenar credenciais no banco de dados. Além disso, a diferenciação de acesso entre alunos e monitores será implementada.



## Arquitetura da solução

1. *Login:*
   - Aluno ou Monitor acessa a página de login.
   - Insere credenciais e faz login no sistema.

2. *Página Inicial:*
   - Após login bem-sucedido, o usuário é redirecionado para a página inicial.
   - Aluno e Monitor têm opções de navegação diferentes.

3. *Aluno:*
   - Acesso à página "Minhas Disciplinas".
   - Visualização das disciplinas disponíveis.
   - Visualização de conteúdo das disciplinas.
   - Acesso à caixa de mensagens para interação com o Monitor no menu lateral.
   - Acesso à página de Ajuda no menu lateral.
   - Logout no menu lateral.

4. *Monitor:*
   - Acesso à página "Adicionar Disciplina".
   - Adição de novas disciplinas ao sistema.
   - Acesso à caixa de mensagens para interação com os Alunos no menu lateral.
   - Acesso à página de Ajuda no menu lateral.
   - Logout.

5. *Mensagens:*
   - Ambos, Aluno e Monitor, podem acessar a caixa de mensagens.
   - Enviar mensagens para os destinatários corretos (Monitor para Alunos ou Alunos para Monitor).
   - Visualizar e responder mensagens recebidas.

6. *Página de Ajuda:*
   - Informações adicionais sobre o funcionamento do site.
   - Instruções sobre como usar diferentes funcionalidades.
   - Links para suporte ou FAQs.
   - Retorno ao menu principal.

7. *Logout:*
   - Encerra a sessão do usuário, redirecionando para a página de login.
  
   
  
Esse diagrama fornece uma representação visual e sequencial das principais funcionalidades do sistema acadêmico, facilitando a compreensão do fluxo de interação entre o usuário e a plataforma.

> **Exemplo do diagrama de Arquitetura**:

![Arquitetura](https://github.com/ICEI-PUC-Minas-PBE-SI/pbe-si-ads-2023-2-tiaw-t2-mentoria/assets/141644522/7fd8f32f-84a6-4b30-aab3-5a0e3d22231b)



# Avaliação da Aplicação

 Cadastro de Alunos e Monitores (RF-001):

Cenário: Verificar se o sistema permite o cadastro correto de alunos e monitores.
Passos:
Acessar a área de cadastro.
Preencher os dados obrigatórios de um aluno.
Preencher os dados obrigatórios de um monitor.
Salvar os cadastros.
Verificar se os dados foram corretamente armazenados no banco de dados.
2. Cadastro de Disciplinas (RF-002):

Cenário: Testar a funcionalidade de cadastro de disciplinas.
Passos:
Acessar a área de administração.
Adicionar uma nova disciplina.
Verificar se a disciplina está listada corretamente.
3. Marcação de Horários com Monitores (RF-003):

Cenário: Testar a marcação de horários entre alunos e monitores.
Passos:
Acessar a agenda.
Escolher uma disciplina.
Selecionar um horário disponível.
Confirmar a marcação.
Verificar se o horário está corretamente agendado.
4. Sistema de Mensagem entre Monitor e Aluno (RF-004):

Cenário: Testar o sistema de mensagens.
Passos:
Enviar mensagem do aluno para o monitor.
Verificar se o monitor recebe a mensagem.
Responder à mensagem do monitor.
Confirmar se o aluno recebe a resposta.
5. Autenticação por Login e Senha (RF-005):

Cenário: Garantir que o sistema permite a entrada apenas com login e senha válidos.
Passos:
Acessar a página de login.
Inserir credenciais corretas.
Verificar o acesso permitido.
Inserir credenciais incorretas.
Verificar a negação de acesso.
6. Compartilhamento de Recursos e Matérias Complementares (RF-006):

Cenário: Testar a funcionalidade de compartilhamento de recursos.
Passos:
Adicionar um recurso.
Compartilhar o recurso com um aluno.
Verificar se o aluno tem acesso ao recurso compartilhado.
7. Encaminhamento para Sites de Feedback (RF-007):

Cenário: Testar o redirecionamento para sites que permitem feedback dos alunos.
Passos:
Clicar no link de feedback.
Verificar se o sistema redireciona corretamente para o site de feedback.
8. Escalabilidade do Sistema (RNF-001):

Cenário: Avaliar como o sistema se comporta com um aumento significativo no número de usuários.
Passos:
Simular o aumento de usuários simultâneos.
Monitorar o desempenho do sistema.
Verificar se o sistema continua responsivo e funcional.
9. Medidas de Segurança (RNF-002):

Cenário: Testar as medidas de segurança implementadas.
Passos:
Tentar acessar dados sem autenticação.
Tentar acessar áreas restritas.
Verificar se medidas de segurança impedem acesso não autorizado.
10. Robustez com Múltiplos Usuários (RNF-003):
- Cenário: Testar a capacidade do sistema de suportar múltiplos usuários simultâneos.
- Passos:
1. Simular múltiplos usuários acessando o sistema simultaneamente.
2. Verificar se o sistema mantém a estabilidade e o desempenho.

11. Responsividade em Dispositivos Móveis (RNF-004):
- Cenário: Verificar se o sistema é responsivo em dispositivos móveis.
- Passos:
1. Acessar o sistema a partir de um dispositivo móvel.
2. Verificar se a interface se ajusta corretamente.

12. Backup Planejado dos Dados (RNF-005):
- Cenário: Testar o processo de backup dos dados.
- Passos:
1. Iniciar o processo de backup manualmente.
2. Verificar se os dados são corretamente salvos.

13. Suporte Técnico (RNF-006):
- Cenário: Avaliar a eficácia do suporte técnico.
- Passos:
1. Simular um problema técnico.
2. Registrar um chamado de suporte.
3. Verificar o tempo de resposta e resolução.

14. Disponibilidade do Sistema (RNF-007):
- Cenário: Verificar se o sistema atende ao requisito de disponibilidade.
- Passos:
1. Monitorar o tempo de atividade do sistema.
2. Verificar se o sistema está disponível 99,9% do tempo, excluindo janelas de manutenção planejada. 



## Plano de Testes

1. *Teste de Autenticação (Login/Logout):*

 *Usuários Envolvidos:* Todos os usuários do sistema.

2. *Teste de Navegação entre Páginas:*
 
 *Usuários Envolvidos:* Todos os usuários do sistema.

3. *Teste de Visualização de Disciplinas:*

*Usuários Envolvidos:* Alunos.

4. *Teste de Adição de Nova Disciplina (para Monitores):*

*Usuários Envolvidos:* Monitores.

5. *Teste de Envio e Recebimento de Mensagens:*

 *Usuários Envolvidos:* Alunos e Monitores.


## Registros de Testes

 1. *Teste de Autenticação (Login/Logout):*
   - *Funcionalidade Avaliada:* Verificamos se o sistema permite que os usuários façam login e logout corretamente. E identificamos que o usuário consegue fazer o login mesmo sem preencher suas credencias, pois o JavaScript ainda não foi desenvolvido para barrar o usuário.

2. *Teste de Navegação entre Páginas:*
   - *Funcionalidade Avaliada:* Identificamos que a navegação entre as diferentes seções do site funciona corretamente.

3. *Teste de Visualização de Disciplinas:*
   - *Funcionalidade Avaliada:* Verificamos que as disciplinas são exibidas corretamente para os alunos.

4. *Teste de Adição de Nova Disciplina (para Monitores):*
   - *Funcionalidade Avaliada:* Testamos que se os monitores conseguem ter acesso a funcionalidade de adicionar novas disciplinas corretamente, na qual é aberto um modal após clicar no botão que permite que o usuário inclua o conteúdo da disciplina que deseja adicionar;

5. *Teste de Envio e Recebimento de Mensagens:*
   - *Funcionalidade Avaliada:* Verificamos se as mensagens são enviadas e recebidas corretamente entre alunos e monitores, e identificamos que ao clicar no botão enviar não temos o retorno esperado, pois não foi desenvolvido o Java Script.


# Referências
FRISON, L. M. B.. (2016). Monitoria: uma modalidade de ensino que potencializa a aprendizagem colaborativa e autorregulada. Pro-posições, 27(1), 133–153. Acesso em 10 Ago 2023, disponivel em: https://doi.org/10.1590/0103-7307201607908

FLATSCHART, Fábio. HTML 5: embarque imediato. Rio de Janeiro: Brasport, 2011.

MARINHO, Antônio Lopes; CRUZ, J. L. Desenvolvimento de aplicações para internet. São Paulo: Pearson Education do Brasil, 2017.

MILETTO, Evandro Manara.; BERTAGNOLLI, Silvia de Castro. Desenvolvimento de software II: introdução ao desenvolvimento web com HTML, CSS, JavaScript e PHP. Porto Alegre: Bookman Editora, 2014.

FLANAGAN, David. JavaScript: o guia definitivo. 6 ed. Porto Alegre: Bookman Editora, 2014.

OLIVEIRA, Cláudio Luís Vieira; ZANETTI, Humberto Augusto Piovesana. Javascript descomplicado: programação para a Web, Iot e dispositivos móveis. São Paulo: Érica, 2020.

SEGURADO, Valquiria Santos (org.).  Projeto de interface com o usuário. Editora Pearson, 2017. ISBN 9788543017303.

TERUEL, Evandro Carlos. HTML 5: guia prático. 2 ed. São Paulo: Érica, 2014.






