<html>
<body>
 <h1 align="center"> API 2º Semestre - 01/2021</h1>
<h1 align="center"> 
<a href="https://github.com/Time-1-ADS/ProjetoGSW/tree/sprints"><img src="https://img.shields.io/badge/GitHub-Repositório Projeto-181717?style=for-the-badge&logo=github"></a>
</h1>
 
 <h2> Parceiro Acadêmico: <a href="https://pqtec.org.br/empresas/gsw/">GSW Soluções Integradas</a></h2>
 
<img src="https://github.com/BryanRibeiro/Portfolio-Projetos/blob/main/images/gsw.png" height="100" width="350"/>
  
  <h2 style="font-family:roboto;"> Resumo do Projeto :clipboard:</h2>
  
  <p align="justify" style="font-family:roboto;"> O projeto tem como objetivo principal desenvolver um Dashboard para a empresa GSW Soluções Integradas, que permitirá a visualização dos status e acompanhamentos dos projetos em andamento. O Dashboard será alimentado por diferentes fontes de dados, agregando informações relevantes e apresentando-as de forma clara e acessível. Através desse Dashboard, a diretoria da empresa poderá ter uma visão abrangente e atualizada do andamento dos projetos, facilitando a análise e tomada de decisões estratégicas. Será possível monitorar o progresso de cada projeto, identificar eventuais desvios, analisar o desempenho de equipes e recursos envolvidos, além de obter métricas e indicadores-chave para avaliar a eficiência e o sucesso dos projetos em diferentes áreas.

 <h2 style="font-family:roboto;"> Tecnologias Adotadas :computer:</h2>
 
 <div style="display: inline_block"><br> 
 <img src="https://raw.githubusercontent.com/devicons/devicon/1119b9f84c0290e0f0b38982099a2bd027a48bf1/icons/postgresql/postgresql-original-wordmark.svg" width="100"    height="100" />	 
 <img src="https://raw.githubusercontent.com/devicons/devicon/1119b9f84c0290e0f0b38982099a2bd027a48bf1/icons/python/python-original-wordmark.svg" width="100"    height="100" />
 <img src="https://raw.githubusercontent.com/devicons/devicon/1119b9f84c0290e0f0b38982099a2bd027a48bf1/icons/javascript/javascript-original.svg" width="100" height="100" />
 <img src="https://raw.githubusercontent.com/devicons/devicon/1119b9f84c0290e0f0b38982099a2bd027a48bf1/icons/html5/html5-original-wordmark.svg" width="100" height="100" />
 <img src="https://raw.githubusercontent.com/devicons/devicon/1119b9f84c0290e0f0b38982099a2bd027a48bf1/icons/css3/css3-original-wordmark.svg" width="100" height="100" />
 <img src="https://raw.githubusercontent.com/devicons/devicon/1119b9f84c0290e0f0b38982099a2bd027a48bf1/icons/visualstudio/visualstudio-plain.svg" width="100" height="100" />
</div>
 
<br>
 
  <ul>
  <li><a href="https://www.postgresql.org/">PostgreSQL</a>: É um sistema de gerenciamento de banco de dados relacional de código aberto, conhecido por sua robustez, confiabilidade e suporte avançado a recursos como transações ACID, replicação e escalabilidade horizontal.</p></li>
  </li>	  
  <li><a href="https://www.python.org/">Python</a>: É uma linguagem de programação de alto nível, interpretada e de propósito geral, conhecida por sua simplicidade, legibilidade e ampla aplicabilidade em diferentes domínios, desde desenvolvimento web até análise de dados.</p></li>
  </li>
   <li><a href="https://developer.mozilla.org/pt-BR/docs/Web/JavaScript">JavaScript</a>: É uma linguagem de programação versátil e poderosa, utilizada para adicionar interatividade, funcionalidades dinâmicas e comportamentos aos sites.</p></li>
  </li>
  <li><a href="https://html.spec.whatwg.org/multipage/">HTML</a>: É uma linguagem de marcação utilizada para estruturar e organizar o conteúdo das páginas da web. Com suas tags e elementos, permite a criação de textos, imagens, links e formulários, fornecendo a base fundamental para a construção de sites. É complementado por outras tecnologias como CSS e JavaScript para estilização e interatividade.</p></li>
  </li>
   <li><a href="https://www.w3.org/Style/CSS/Overview.en.html">CSS</a>: É uma linguagem de estilo utilizada para definir a apresentação e o layout visual das páginas da web.</p></li>
  </li>
  <li><a href="https://trello.com/https://trello.com">Visual Studio Code</a>: É um editor de código-fonte leve e altamente personalizável, desenvolvido pela Microsoft, com suporte a várias linguagens de programação e uma ampla gama de extensões que aumentam sua funcionalidade.</p></li>
  </li>

  </ul>
  
  <h2 style="font-family:roboto;"> Contribuições Individuais :dart:</h2>
  
  <h3> Atribuições como Desenvolvedor Front-end</h3>
 
 Na parte das tasks do projeto do Dashboard, como desenvolvedor front-end, eu contribuí não apenas com o código CSS, mas também com o desenvolvimento das tasks em geral, utilizando JavaScript e integrando-o ao HTML e CSS. Implementei funcionalidades interativas nas tasks, como adicionar, editar, excluir e marcar como concluídas. Trabalhei com o JavaScript, manipulando os elementos da página e respondendo aos eventos do usuário, como cliques em botões ou submissões de formulários.
 
 <details>
	
<summary>Código em CSS - Classes para as tasks do Dashboard</summary>
 
 ```css
 
 body{
    background: #ECEDF3;
    margin: 0px;
    display: flex;
    align-items: flex-start;
    flex-direction: column;
    overflow: hidden;
}
h1{
    color: #F8F9FC;
    font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
    font-size: 35px;
}
.container-top {
    height: 770px;
    background: #25408F;
}

.bvoltar{
    background: #ECEDF3;
    border-radius: 20px;
    border: 0px;
    width: 80px;
    height: 25px;
    display: flex;
    align-items:flex-end;
    justify-content:space-between;
    box-shadow: 2px 2px 2px #022f58;
}

.block1{
    background: #F8F9FC;
    border-radius: 15px;
    box-shadow: 2px 2px 2px #c7c8ce;
    justify-content: center;
    min-height: 480px;
    max-height: 480px;
}

.titulos{
    display: flex;
    align-items: center;
    justify-content: center;
    background: #25408F;
    border-radius: 25px;
    color: white;
    font-size: 28px;
}

.titulos2{
    display: flex;
    align-items: center;
    justify-content: center;
    background: #1CC88A;
    border-radius: 25px;
    color: white;
    font-size: 28px;
}

.titulos3{
    display: flex;
    align-items: center;
    justify-content: center;
    background: #E74A3B;
    border-radius: 25px;
    color: white;
    font-size: 28px;
}




.estilo{
    font-family: Arial, Helvetica, sans-serif;
    font-style: normal;
    font-weight: bold;
    font-size: 30px;
    color: white;
    
}

.section-content{
    font-family: Arial, Helvetica, sans-serif;
    font-style: normal;
    font-size: 14px;
    min-height: 40px;
    color: black;
}

.estilo2{
    font-family: Arial, Helvetica, sans-serif;
    font-style: normal;
    font-size: 18px;
    color: black;
    justify-content: center;
    display: flex;
    margin-top: 40px;

}


#style-8::-webkit-scrollbar-track
{
	-webkit-box-shadow: inset 0 0 6px rgba(0,0,0,0.3);
	background-color: #F5F5F5;
	border-radius: 10px;
}

#style-8::-webkit-scrollbar
{
	width: 10px;
	background-color: #F5F5F5;
}

#style-8::-webkit-scrollbar-thumb
{
	border-radius: 10px;
	background-image: -webkit-gradient(linear,
									   left bottom,
									   left top,
									   color-stop(0.44, rgb(122,153,217)),
									   color-stop(0.72, rgb(73,125,189)),
									   color-stop(0.86, rgb(28,58,148)));
}


.search_icon{
    color: #010308;
    display: flex;
}

.search-input {
    border-radius: 50px !important;
}


.form-outline{
    display: flex;
    border-radius: 12.5px;
    background: #ECEDF3;
    box-shadow: 2px 2px 2px #022f58;
}

.form-control{
    border-radius: 12.5px;
    border: 0px;
    height: 25px;
    width: 210px;
    margin-left: 20px;
    background: #ECEDF3;
}
 
 ```
 
 </details>  
 
Busquei dados das tasks em uma fonte de dados externa, como um banco de dados ou uma API, utilizando o JavaScript. Esses dados foram apresentados dinamicamente no Dashboard, permitindo a exibição atualizada das informações das tasks. Em termos de integração com o CSS, utilizei classes ou IDs dinâmicos no JavaScript para aplicar estilos específicos a determinados elementos ou alterar a aparência das tasks com base em seu estado (por exemplo, alterar a cor ou adicionar um indicador visual para tarefas concluídas).
 
Trabalhei no desenvolvimento de um código JavaScript que permitiu tornar o Dashboard responsivo, ou seja, adaptável a diferentes tamanhos de tela e dispositivos. Utilizei técnicas como media queries para identificar o tamanho da tela do usuário e aplicar estilos adequados para cada tamanho, garantindo uma experiência visual agradável em dispositivos móveis, tablets e desktops. Fui responsável pela criação e funcionalidade do menu lateral das tasks. Utilizando JavaScript, implementei um menu interativo que se expandia e recolhia conforme a interação do usuário. Isso proporcionou uma navegação intuitiva e organizada entre as diferentes seções do Dashboard.
 
 <details>
	
<summary>Código em JavaScript - Responsividade e Menu Lateral</summary>
 
 ```javascript
 
 var ctx1 = document.getElementById('TaskGeral').getContext('2d');

fetch('https://apigsw.herokuapp.com/data/task/')
    .then(function (response) {
        return response.json();
    })
    .then(function (dados) {
        var chart = new Chart(ctx1, {
            type: 'doughnut',
            data: {

                labels: ['Fechada', 'Aberta'],
                datasets: [{
                    label: 'Tasks',
                    backgroundColor: [
                        'rgba(231, 74, 59)',
                        'rgba(28, 200, 138)'
                    ],
                    borderColor: [
                        'rgba(231, 74, 59)',
                        'rgba(28, 200, 138)'
                    ],
                    data: [(dados[1][1]), (dados[2][1])],
                }]
            },
        });
    });
 
 ```
 
 </details> 

Ao clicar em um item do menu, eu também desenvolvi a lógica necessária para exibir as informações correspondentes às tasks relacionadas na área de conteúdo principal do Dashboard. Isso envolveu a manipulação do DOM (Document Object Model) para adicionar ou remover elementos dinamicamente e atualizar as informações exibidas conforme a seleção do usuário.
 
  <h3> Atribuições como Scrum Master</h3>
  <p align="justify" style="font-family:roboto;"> As atribuições como Scrum Master da equipe foram pertinentes a realizar um bom planejamento e organização das ações do grupo no decorrer das Sprints. No início do projeto foi realizada uma reunião para definir nosso principal meio de comunicação e a ferramenta para monitoramento de tarefas, assim decidimos utilizar, respectivamente, o Discord e GitHub Projects. Como Master da equipe, fiquei responsável por acompanhar e analisar o progresso do grupo nesses softwares, de modo a observar se todos os integrantes estavam participando das reuniões semanais e se apresentavam alguma dificuldade com a evolução das tarefas, logo atuando da melhor maneira de acordo com a situação.</p>

 <details>
      <summary>Cards das Sprints</summary>
<h1 align="center"> <img src = "https://github.com/Time-1-ADS/ProjetoGSW/blob/sprints/Imagens%20Geral/cardsgit.png" /></h1>
 
 </details> 

<p align="justify" style="font-family:roboto;"> Após a apresentação do problema por parte do cliente, nos reunimos para a elaboração de um Backlog conciso com as necessidades do cliente. Obtendo como resultado final desse processo as User Stories que compõe o Product Backlog e a descrição da experiência do usuário com o produto, além de promover um ótimo entendimento das regras de negócio e os primeiros questionamentos para o cliente. Com esse alinhamento inicial finalizado, as User Stories foram divididas entre as 4 Sprints do projeto, dessa forma tive a função de quebrar essas histórias em tarefas menores e mais objetivas, para um melhor desenvolvimento do que foi planejado, e também delegar essas tasks entre os integrantes da equipe.</p>

  <h2 style="font-family:roboto;"> Funcionamento :bulb:</h2>

  <h1 align="center"> <img src = "https://github.com/Time-1-ADS/ProjetoGSW/blob/sprints/Imagens%20Geral/dashboard4.gif"/></h1>
 
  <h2 style="font-family:roboto;"> Aprendizados Efetivos :book:</h2>  
  
Durante o desenvolvimento desse projeto de criação do Dashboard para a empresa GSW Soluções Integradas, pude adquirir diversos aprendizados significativos que contribuíram para o meu crescimento e desenvolvimento como desenvolvedor.

Este projeto me proporcionou a oportunidade de aprofundar meus conhecimentos em visualização de dados e desenvolvimento de painéis de controle. Aprendi a selecionar e utilizar as ferramentas certas para apresentar as informações de forma clara e acessível, garantindo que a diretoria da empresa possa obter insights valiosos sobre o andamento dos projetos. Isso envolveu o uso de bibliotecas e frameworks especializados, bem como a compreensão de princípios de design visual e organização de dados.

Além disso, trabalhar com diferentes fontes de dados foi um desafio enriquecedor. Aprendi a integrar e consolidar informações provenientes de diversas fontes, como sistemas de gerenciamento de projetos, bases de dados internas e APIs externas. Compreender como manipular e transformar esses dados em um formato adequado para serem apresentados no Dashboard foi uma habilidade valiosa adquirida durante o projeto.
  
  <h3 align="center"> Hard Skills </h3>
  <table align="center">
    <tr>
      <th width="280px">Tecnologia/Metodologia</th>
      <th width="85px">Nota</th>
      <th width="240px">Classificação</th>
    </tr>
    <tr>
      <td>Metodologia Scrum - Scrum Master</td>
      <td>★★★★☆</td>
	<td>Sei fazer com ajuda</td>
    </tr>
    <tr>
      <td>PostgreSQL</td>
      <td>★★★☆☆</td>
	<td>Entendi</td>
    </tr>	
    <tr>
      <td>Python</td>
      <td>★★★☆☆</td>
	<td>Entendi</td>
    </tr>
    <tr>
      <td>JavaScript</td>
      <td>★★★☆☆</td>
	<td>Entendi</td>
    </tr>
   <tr>
      <td>HTML</td>
      <td>★★★★★</td>
	<td>Sei fazer com autonomia</td>
    </tr>
   <tr>
      <td>CSS</td>
      <td>★★★★☆</td>
	<td>Sei fazer com ajuda</td>
    </tr>
    <tr>
      <td>Visual Studio Code</td>
      <td>★★★★☆</td>
	<td>Sei fazer com ajuda</td>
    </tr>
  </table>
  
  <h3 align="center">Soft Skills</h3>
  <table align="center">
    <tr>
      <th width="270px">Habilidade</th>
      <th width="290px">Descrição</th>
    </tr>
    <tr>
      <td>Responsabilidade</td>
      <td>Assumi o cargo de Scrum Master pela primeira vez.</td>
    </tr>
<tr>
  <td>Liderança Servidora</td>
  <td>Desenvolvi habilidades de liderança servidora, facilitando o sucesso da equipe e removendo obstáculos.</td>
</tr>
<tr>
  <td>Facilitação de Eventos</td>
  <td>Aprimorei minhas técnicas de facilitação, garantindo a eficácia dos eventos do Scrum, como Daily Standups e Retrospectives.</td>
</tr>
<tr>
  <td>Resolução de Conflitos</td>
  <td>Lidei com conflitos de equipe de forma proativa, promovendo um ambiente colaborativo e positivo.</td>
</tr>
<tr>
  <td>Melhoria Contínua</td>
  <td>Implementei práticas para aprimorar continuamente os processos e a eficácia do time, baseando-me em retrospectivas.</td>
</tr>
<tr>
  <td>Coaching</td>
  <td>Desenvolvi habilidades de coaching para apoiar o crescimento individual dos membros da equipe.</td>
</tr>
  </table>
  
---

 <h2 align="center"> Navegação Projetos :link:</h2>
 
   <p align="justify" style="font-family:roboto;"><li><a href="https://github.com/BryanRibeiro/Portfolio-Projetos/blob/main/API_1.md">1º Semestre: SOS EDUCA - Site de Vendas de Materiais Didáticos.</a></li></p>
   <p align="justify" style="font-family:roboto;"><li>2º Semestre: GSW - Dashboard para acompanhamentos dos projetos, através de diferentes fontes de dados.</a></li></p>
   <p align="justify" style="font-family:roboto;"><li><a href="https://github.com/BryanRibeiro/Portfolio-Projetos/blob/main/API_3.md">3° Semestre: PromoAll - Ecommerce com um motor de regras para promoções aplicadas no momento da compra.</a></li></p>
   <p align="justify" style="font-family:roboto;"><li><a href="https://github.com/BryanRibeiro/Portfolio-Projetos/blob/main/API_4.md">4° Semestre: Subiter - Aplicação Web para sincronização dos dados administrativos, financeiros e operacionais.</a></li></p>
   <p align="justify" style="font-family:roboto;"><li><a href="https://github.com/BryanRibeiro/Portfolio-Projetos/blob/main/API_5.md">5º Semestre: Tech Ninjas - Automatização de transferência de arquivos entre nuvens.</a></li></p>
   <p align="justify" style="font-family:roboto;"><li><a href="https://github.com/BryanRibeiro/Portfolio-Projetos/blob/main/API_6.md">6º Semestre: Tech Vision - Sistema de Informação Geográfica de dados públicos do ProAgro.</a></li></p>
  
</body>
</html>
