<html>
<body>
 <h1 align="center"> API 1º Semestre - 02/2020</h1>
<a href="https://github.com/Grupo-1-2020-PI-FATEC-ADS/SOS-EDUCA"><img src="https://img.shields.io/badge/GitHub-Repositório Projeto-181717?style=for-the-badge&logo=github"></a>
 
 <h2> Parceiro Acadêmico: <a href="https://fatecsjc-prd.azurewebsites.net/">FATEC São José dos Campos - Prof. Jessen Vidal</a></h2>
 
<img src="https://github.com/BryanRibeiro/Portfolio-Projetos/blob/main/images/fatecsjc_400x192.png" height="100" width="230"/>
  
  <h2 style="font-family:roboto;"> Resumo do Projeto :clipboard:</h2>
  
  <p align="justify" style="font-family:roboto;"> O projeto consiste na criação de um site de comércio eletrônico (E-commerce) voltado para materiais didáticos. O objetivo principal foi facilitar o acesso e fornecer recursos de qualidade para professores e alunos, com o intuito de apoiar seus estudos e aprimorar o processo de aprendizagem. O site oferece uma ampla variedade de materiais didáticos, abrangendo diversas disciplinas e níveis educacionais. Isso inclui livros, apostilas, e-books, vídeos educativos, planos de aula, jogos educativos, entre outros recursos relevantes para auxiliar tanto os educadores quanto os estudantes.
Uma das principais características do site foi a facilidade de navegação e busca, permitindo que os usuários encontrem rapidamente o conteúdo desejado. Além disso, fornecer recursos de filtragem e classificação, permitindo que os usuários refinem suas pesquisas com base em critérios específicos, como disciplina, nível de ensino, autor, editora, entre outros.
   
  <p align="justify" style="font-family:roboto;"> As funcionalidades desenvolvidas no site foram: 
 </p>
  <ul>
<li>Login/Cadastro de usuário;</li>
<li>Área do Administrador para análise das vendas;</li>
<li>Área do Cliente com acompanhamento das compras;</li>
<li>Carrinho de Compras;</li>
<li>Saldo de Créditos;</li>
<li>Relatório de Vendas;</li>
<li>Pagamento via Cartão;</li>
<li>Pagamento via Boleto;</li>
<li>Acessibilidade (Libras).</li>
  </ul>
 </p>
 
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
  
  <h3> Atribuições como Desenvolvedor Front-end</h3>
  <p align="justify" style="font-family:roboto;"> Como desenvolvedor front-end nesse projeto, minhas atribuições foram as seguintes:

**Design responsivo:** Eu fui responsável por criar um layout responsivo que se adaptasse a diferentes dispositivos e tamanhos de tela. Isso permitiu que os usuários acessassem o site de qualquer dispositivo, como computadores, tablets e smartphones, proporcionando uma experiência consistente e agradável.

<details>
	
<summary>Código PHP - Exemplo</summary>
 
```php
 
$conn = mysqli_connect("localhost", "usuario", "senha", "banco_de_dados");

$query = "SELECT * FROM produtos";
$result = mysqli_query($conn, $query);

while ($row = mysqli_fetch_assoc($result)) {
  
 // Informações do produto
  echo "<div class='product'>";
  echo "<h3>" . $row['titulo'] . "</h3>";
  echo "<p>" . $row['descricao'] . "</p>";
  echo "</div>";
}

mysqli_close($conn);
?>
 
```
 
O código acima é um exemplo simples do que fizemos utilizando o PHP para exibir os produtos do site. Ele realiza uma consulta ao banco de dados e exibe as informações dos produtos em um loop.
 
</details> 
 
**Implementação da interface de usuário:** Ajudei a traduzir os designs de interface fornecidos pela equipe de design em código HTML, CSS e JavaScript. Isso envolveu a criação de páginas web interativas e funcionais, incluindo a exibição de produtos, páginas de detalhes do produto, carrinho de compras e formulários de pagamento.
 
<details>
	
<summary>Código HTML - Exemplo</summary>
 
```html
 
// Exemplo de integração com a API de pagamento
function fazerPagamento(total, dadosPagamento) {
  // Chamada para a API de pagamento
  fetch('https://api.paymentprovider.com/payment', {
    method: 'POST',
    headers: {
      'Content-Type': 'application/json',
    },
    body: JSON.stringify(dadosPagamento),
  })
    .then(response => response.json())
    .then(data => {
      // Processar a resposta da API de pagamento
      if (data.status === 'success') {
        // Pagamento realizado com sucesso
        // Executar ações adicionais, como atualizar o status do pedido, exibir uma mensagem de sucesso, etc.
      } else {
        // O pagamento falhou
        // Lidar com o erro, exibir uma mensagem de erro, etc.
      }
    })
    .catch(error => {
      // Ocorreu um erro na chamada para a API de pagamento
      // Lidar com o erro, exibir uma mensagem de erro, etc.
    });
}

// Exemplo de integração com a API de entrega
function realizarEntrega(endereco, dadosEntrega) {
  // Chamada para a API de entrega
  fetch('https://api.deliveryprovider.com/delivery', {
    method: 'POST',
    headers: {
      'Content-Type': 'application/json',
    },
    body: JSON.stringify(dadosEntrega),
  })
    .then(response => response.json())
    .then(data => {
      // Processar a resposta da API de entrega
      if (data.status === 'success') {
        // Entrega realizada com sucesso
        // Executar ações adicionais, como atualizar o status do pedido, exibir uma mensagem de sucesso, etc.
      } else {
        // A entrega falhou
        // Lidar com o erro, exibir uma mensagem de erro, etc.
      }
    })
    .catch(error => {

    });
}
 
```
 
</details> 

**Integração com APIs:** Trabalhei na integração do front-end com as APIs fornecidas pelos serviços externos, como sistemas de pagamento, serviços de entrega e gerenciamento de estoque. Isso permitiu que os usuários realizassem transações de compra de forma segura e eficiente, além de receberem atualizações sobre o status dos pedidos.

**Otimização de desempenho:** Otimizei o desempenho do site, garantindo que as páginas carregassem rapidamente e que o código fosse eficiente. Isso incluiu a minificação e concatenação de arquivos CSS e JavaScript, otimização de imagens e implementação de técnicas de cache.
</p>
  
  
  <h2 style="font-family:roboto;"> Funcionamento :bulb:</h2>

  <h1 align="center"> <img src = "https://github.com/Grupo-1-2020-PI-FATEC-ADS/SOS-EDUCA/blob/master/Imagens%20Geral/videosprint3.gif"/></h1>
 
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
   <p align="justify" style="font-family:roboto;"><li><a href="https://github.com/BryanRibeiro/Portfolio-Projetos/blob/main/API_5.md">5º Semestre: MidAll - Transferência automática de arquivos entre nuvens e análise dos metadados.</a></li></p>
   <p align="justify" style="font-family:roboto;"><li><a href=""> 6º Semestre: Em Construção 🏗️</a></li></p>
  
</body>
</html>
