<html>
<body>
 <h1 align="center"> API 3º Semestre - 01/2022</h1>
<a href="https://github.com/Time-1-ADS/ProjetoGSW/tree/sprints"><img src="https://img.shields.io/badge/GitHub-Repositório Projeto-181717?style=for-the-badge&logo=github"></a>
 
 <h2> Parceiro Acadêmico: <a href="https://pqtec.org.br/empresas/gsw/">GSW Soluções Integradas</a></h2>
 
<img src="https://github.com/BryanRibeiro/Portfolio-Projetos/blob/main/images/gsw.png" height="100" width="350"/>
  
  <h2 style="font-family:roboto;"> Resumo do Projeto :clipboard:</h2>
  
  <p align="justify" style="font-family:roboto;"> O projeto tem como objetivo principal desenvolver um Dashboard para a empresa GSW Soluções Integradas, que permitirá a visualização dos status e acompanhamentos dos projetos em andamento. O Dashboard será alimentado por diferentes fontes de dados, agregando informações relevantes e apresentando-as de forma clara e acessível.

Através desse Dashboard, a diretoria da empresa poderá ter uma visão abrangente e atualizada do andamento dos projetos, facilitando a análise e tomada de decisões estratégicas. Será possível monitorar o progresso de cada projeto, identificar eventuais desvios, analisar o desempenho de equipes e recursos envolvidos, além de obter métricas e indicadores-chave para avaliar a eficiência e o sucesso dos projetos em diferentes áreas.

 <h2 style="font-family:roboto;"> Tecnologias Adotadas :computer:</h2>
 
 <div style="display: inline_block"><br> 
 <img src="https://raw.githubusercontent.com/devicons/devicon/1119b9f84c0290e0f0b38982099a2bd027a48bf1/icons/mysql/mysql-original-wordmark.svg" width="100"    height="100" />	 
 <img src="https://raw.githubusercontent.com/devicons/devicon/1119b9f84c0290e0f0b38982099a2bd027a48bf1/icons/html5/html5-original-wordmark.svg" width="100"    height="100" />
 <img src="https://raw.githubusercontent.com/devicons/devicon/1119b9f84c0290e0f0b38982099a2bd027a48bf1/icons/css3/css3-original-wordmark.svg" width="100" height="100" />
 <img src="https://raw.githubusercontent.com/devicons/devicon/1119b9f84c0290e0f0b38982099a2bd027a48bf1/icons/php/php-plain.svg" width="100" height="100" />
 <img src="https://raw.githubusercontent.com/devicons/devicon/1119b9f84c0290e0f0b38982099a2bd027a48bf1/icons/trello/trello-plain-wordmark.svg" width="100" height="100" />
</div>
 
<br>
 
  <ul>
  <li><a href="https://www.mysql.com/">MySQL</a>: MySQL é um sistema de gerenciamento de banco de dados (SGBD) relacional, ou seja, que utiliza a linguagem SQL como interface. Lançado sobre a licença GPL, possui como desenvolvedor a Oracle Corporation.</p></li>
  </li>	  
  <li><a href="https://html.spec.whatwg.org/multipage/">HTML</a>: É uma linguagem de marcação utilizada para estruturar e organizar o conteúdo das páginas da web. Com suas tags e elementos, permite a criação de textos, imagens, links e formulários, fornecendo a base fundamental para a construção de sites. É complementado por outras tecnologias como CSS e JavaScript para estilização e interatividade.</p></li>
  </li>
   <li><a href="https://www.w3.org/Style/CSS/Overview.en.html">CSS</a>: CSS é uma linguagem de estilo utilizada para definir a apresentação e o layout visual das páginas da web.</p></li>
  </li>
   <li><a href="https://www.php.net/">PHP</a>: É uma linguagem de programação server-side amplamente utilizada para desenvolvimento web. Com sua sintaxe simples e poderosa, permite a criação de sites dinâmicos, interativos e conectados a bancos de dados, possibilitando a construção de aplicativos web robustos.</p></li>
  </li>
   <li><a href="https://developer.mozilla.org/pt-BR/docs/Web/JavaScript">JavaScript</a>: É uma linguagem de programação versátil e poderosa, utilizada para adicionar interatividade, funcionalidades dinâmicas e comportamentos aos sites.</p></li>
  </li>
  <li><a href="https://trello.com/https://trello.com">Trello</a>: Foi utilizado como ferramenta do método Scrum para distribuição das atividades do grupo e priorização das demandas. Possibilitando realizar o planejamento das sprints, sendo capaz de registrar o progresso da equipe e do projeto, facilitando o desenvolvimento e acompanhamento da realização de tarefas. </p></li>
  </li>

  </ul>
  
  <h2 style="font-family:roboto;"> Contribuições Individuais :dart:</h2>
  
  <h3> Atribuições como Desenvolvedor Back-end e Front-end</h3>
  <p align="justify" style="font-family:roboto;"> Como desenvolvedor nesse projeto, minhas atribuições foram essenciais para a implementação das interfaces do usuário e para garantir uma experiência de usuário fluida e amigável.

Minha contribuição utilizando PHP permitiu a implementação da funcionalidade de autenticação de usuários, a persistência de dados por meio de variáveis de sessão e o reaproveitamento de código com a inclusão de arquivos PHP. Essas contribuições foram essenciais para o bom funcionamento e segurança do sistema de login do cliente no projeto.

<details>
	
<summary>Manipulação dos dados com PHP</summary>
 
> Inicialização de sessão: Com a linha "?php session_start(); ?", iniciei uma sessão PHP. Isso permite que armazene e acesse variáveis de sessão, que podem ser usadas para manter dados específicos do usuário entre as requisições.

> Utilizei o PHP para manipular os dados submetidos no formulário de login. O formulário é enviado para o arquivo "autenticando_clientes.php" através do atributo action no elemento "form".
	
```php
 
<?php session_start(); ?>
<!DOCTYPE html>
<html lang="pt-br">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <?php include('cabecalho.php');?>
	<title>Login do cliente</title>
</head>
<body>
  <?php include('navbar.php');?>
  <?php (include("progresso.php"))(1);?>
 
  <div class="container">
	<!-- Main Content -->
	<div class="container-fluid">
		<div class="row main-content bg-success text-center">
			<div class="col-md-4 text-center company__info">
				<span class="company__logo"><h2><img src="images/sos.gif" alt="" width="120px" height="120px"></span></h2></img>
			</div>
			<div class="col-md-8 col-xs-12 col-sm-12 login_form ">
				<div class="container-fluid">
					<div class="row">
						<h2>Log In</h2>
					</div>
					<div class="row">
						<form control="" class="form-group" action="autenticando_clientes.php" method="POST">
							<div class="row">
								<input type="text" id="username" class="form__input" name="usuario" value="<?php echo @$_SESSION['usuario']?>"  placeholder="Digite seu Email">
							</div>
							<div class="row">
								<!-- <span class="fa fa-lock"></span> -->
								<input type="password" id="password" class="form__input" name="senha" <?= @$_SESSION['senha'] ? 'autofocus' : '' ?>  maxlength="8" placeholder="Digite sua senha">
							</div>
							<div class="row">
								<input type="submit" value="Login" class="btn2">
							</div>
						</form>
					</div>
				</div>
			</div>
		</div>
  </div>
</div>
</body>
  <?php include('rodape.php');?> 
</body>
</html>

```

</details>  

<details>
	
<summary>Validação do Formulário de Login</summary>
 
```javascript

document.getElementById("loginForm").addEventListener("submit", function(event) {
  event.preventDefault();
  var email = document.getElementById("email").value;
  var password = document.getElementById("password").value;
  
  // Realizar validação do email e senha
  if (email && password) {
    // Fazer chamada assíncrona para o backend em PHP
    fetch("login.php", {
      method: "POST",
      body: JSON.stringify({ email: email, password: password }),
      headers: {
        "Content-Type": "application/json"
      }
    })
    .then(response => response.json())
    .then(data => {
      // Tratar a resposta do backend
    })
    .catch(error => {
      // Tratar erros
    });
  }
});

```

</details>  
 
**Criação e Estilização de Interfaces:**
Desenvolvi as interfaces do usuário utilizando HTML, CSS e Bootstrap, seguindo as diretrizes de design fornecidas pelo Figma como referência.
Ajudei a criar um layout responsivo que se adaptasse a diferentes dispositivos e tamanhos de tela. Isso permitiu que os usuários acessassem o site de qualquer dispositivo, como computadores, tablets e smartphones, proporcionando uma experiência consistente.
Ao utilizar o Bootstrap, aproveitei os componentes e classes pré-definidos para criar rapidamente interfaces consistentes, economizando tempo e esforço.

<details>
	
<summary>Estilização do formulário de Login</summary>
	
```css

  .wrapper {
    display: flex;
    align-items: center;
    flex-direction: column; 
    justify-content: center;
    width: 100%;
    min-height: 100%;
    padding: 20px;
  }
  
  #formContent {
    -webkit-border-radius: 10px 10px 10px 10px;
    border-radius: 10px 10px 10px 10px;
    background: #fff;
    padding: 30px;
    width: 90%;
    max-width: 450px;
    position: relative;
    padding: 0px;
    -webkit-box-shadow: 0 30px 60px 0 rgba(0,0,0,0.3);
    box-shadow: 0 30px 60px 0 rgba(0,0,0,0.3);
    text-align: center;
  }
  
  #formFooter {
    background-color: #f6f6f6;
    border-top: 1px solid #dce8f1;
    padding: 25px;
    text-align: center;
    -webkit-border-radius: 0 0 10px 10px;
    border-radius: 0 0 10px 10px;
  }

```
 
</details> 
  
  <h2 style="font-family:roboto;"> Funcionamento :bulb:</h2>

  <h1 align="center"> <img src = "https://github.com/Time-1-ADS/ProjetoGSW/blob/sprints/Imagens%20Geral/dashboard4.gif"/></h1>
 
  <h2 style="font-family:roboto;"> Aprendizados Efetivos :book:</h2>   
  <h3 align="center"> Hard Skills </h3>
  <table align="center">
    <tr>
      <th width="300px">Tecnologia/Metodologia</th>
      <th width="300px">Classificação</th>
    </tr>
    <tr>
      <td>Metodologia Ágil Scrum</td>
      <td>★★☆☆☆</td>
    </tr>
    <tr>
      <td>MySQL</td>
      <td>★★★☆☆</td>
    </tr>	
    <tr>
      <td>HTML</td>
      <td>★★★★☆</td>
    </tr>
    <tr>
      <td>CSS</td>
      <td>★★★★☆</td>
    </tr>
   <tr>
      <td>PHP</td>
      <td>★★★☆☆</td>
    </tr>
   <tr>
      <td>JavaScript</td>
      <td>★★☆☆☆</td>
    </tr>
    <tr>
      <td>GIT</td>
      <td>★★★☆☆</td>
    </tr>
  </table>
  
  <h3 align="center">Soft Skills</h3>
  <table align="center">
    <tr>
      <th width="300px">Habilidade</th>
      <th width="300px">Descrição</th>
    </tr>
    <tr>
      <td>Proatividade</td>
      <td>Precisei estudar bastante sobre desenvolvimento web.</td>
    </tr>
    <tr>
      <td>Conhecimento</td>
      <td>Precisei aprender a utilizar e aplicar o Scrum no projeto.</td>
    </tr>
    <tr>
      <td>Comunicação</td>
      <td>Precisei me comunicar sobre a evolução das minhas tarefas.</td>
    </tr>
    <tr>
      <td>Organização</td>
      <td>Precisei organizar a documentação e código no GitHub.</td>
    </tr>
  </table>
  
---

 <h2 align="center"> Navegação Projetos :link:</h2>
 
   <p align="justify" style="font-family:roboto;"><li> 1º Semestre: SOS EDUCA - Site de Vendas de Materiais Didáticos</li></p>
   <p align="justify" style="font-family:roboto;"><li><a href="https://github.com/BryanRibeiro/Portfolio-Projetos/blob/main/API_2.md">2º Semestre: GSW - Dashboard para acompanhamentos dos projetos, através de diferentes fontes de dados.</a></li></p>
   <p align="justify" style="font-family:roboto;"><li><a href="https://github.com/BryanRibeiro/Portfolio-Projetos/blob/main/API_3.md">3° Semestre: PromoAll - Ecommerce com um motor de regras para promoções aplicadas no momento da compra.</a></li></p>
   <p align="justify" style="font-family:roboto;"><li><a href="https://github.com/BryanRibeiro/Portfolio-Projetos/blob/main/API_4.md">4° Semestre: Subiter - Aplicação Web para sincronização dos dados administrativos, financeiros e operacionais.</a></li></p>
   <p align="justify" style="font-family:roboto;"><li><a href="https://github.com/BryanRibeiro/Portfolio-Projetos/blob/main/API_5.md">5º Semestre: Em Construção 🏗️</a></li></p>
   <p align="justify" style="font-family:roboto;"><li><a href="https://github.com/BryanRibeiro/Portfolio-Projetos/blob/main/API_6.md">6º Semestre: Em Construção 🏗️</a></li></p>
  
</body>
</html>
