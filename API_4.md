<html>
<body>
 <h1 align="center"> API 4º Semestre - 02/2022</h1>
<a href="https://github.com/Doc-Docker/APIMidAll"><img src="https://img.shields.io/badge/GitHub-Repositório Projeto-181717?style=for-the-badge&logo=github"></a>
 
 <h2> Parceiro Acadêmico: <a href="https://midall.com.br/">MidAll [B]</a></h2>
 
<img src="https://github.com/BryanRibeiro/Portfolio-Projetos/blob/main/images/logo%20midall.png" height="150" width="230"/>
  
  <h2 style="font-family:roboto;"> Resumo do Projeto :clipboard:</h2>
  
  <p align="justify" style="font-family:roboto;"> O projeto visa resolver o problema da empresa MidAll relacionado à criação de promoções em seu e-commerce. A solução proposta foi desenvolver um mini motor de regras que permitiu a flexibilidade e rápida atualização das mecânicas das promoções no sistema. Isso foi feito por meio de uma interface onde as regras das promoções poderiam ser cadastradas e aplicadas automaticamente quando os itens fossem adicionados ao carrinho de compras. Essa abordagem ofereceu agilidade na configuração e adaptação das promoções, proporcionando uma experiência personalizada aos clientes.

**O problema é:** O cliente tem um e-commerce, porém necessita de um sistema de compras inteligente que gere promoções com base nas vendas;

**Que afeta** as compras feitas pelos clientes no site;

**O impacto disto é** gerar mais vendas e lucros para a empresa, para que o cliente final fique satisfeito com suas promoções;

**A solução seria** O desenvolvimento de uma aplicação web que irá automatizar este processo no ato da compra, gerando promoções específicas.

<h2 style="font-family:roboto;"> Tecnologias Adotadas :computer:</h2>
 
 <div style="display: inline_block"><br> 
 <img src="https://github.com/devicons/devicon/blob/master/icons/microsoftsqlserver/microsoftsqlserver-plain-wordmark.svg" width="100"    height="100" />	 
 <img src="https://raw.githubusercontent.com/devicons/devicon/1119b9f84c0290e0f0b38982099a2bd027a48bf1/icons/java/java-original-wordmark.svg" width="100"    height="100" />
 <img src="https://raw.githubusercontent.com/devicons/devicon/1119b9f84c0290e0f0b38982099a2bd027a48bf1/icons/angularjs/angularjs-original.svg" width="100" height="100" />
 <img src="https://raw.githubusercontent.com/devicons/devicon/1119b9f84c0290e0f0b38982099a2bd027a48bf1/icons/css3/css3-original-wordmark.svg" width="100" height="100" />
 <img src="https://raw.githubusercontent.com/devicons/devicon/1119b9f84c0290e0f0b38982099a2bd027a48bf1/icons/bootstrap/bootstrap-original-wordmark.svg" width="100" height="100" />
 <img src="https://raw.githubusercontent.com/devicons/devicon/1119b9f84c0290e0f0b38982099a2bd027a48bf1/icons/figma/figma-original.svg" width="100" height="100" />
</div>
 
<br>
 
  <ul>
  <li><a href="https://azure.microsoft.com/">Microsoft SQL Server</a>: O Microsoft SQL Server é um sistema de gerenciamento de banco de dados relacional desenvolvido pela Microsoft, amplamente utilizado para armazenar, manipular e recuperar dados de forma eficiente e segura.</p></li>
  </li>	  
  <li><a href="https://www.java.com/pt-BR/">Java</a>: Java é uma linguagem de programação de alto nível, multiplataforma e orientada a objetos, conhecida por sua portabilidade e segurança, amplamente usada no desenvolvimento de aplicativos e sistemas corporativos.</p></li>
  </li>
   <li><a href="https://angular.io/">Angular</a>: É um framework de desenvolvimento de aplicativos web de código aberto, baseado em TypeScript, que permite a criação de interfaces de usuário dinâmicas e escaláveis, utilizando conceitos como componentes e injeção de dependência.</p></li>
  </li>
   <li><a href="https://www.w3.org/Style/CSS/Overview.en.html">CSS</a>: CSS é uma linguagem de estilo utilizada para definir a apresentação e o layout visual das páginas da web.</p></li>
  </li>
   <li><a href="https://getbootstrap.com/">Bootstrap</a>: Bootstrap é um framework front-end de código aberto que facilita o desenvolvimento de interfaces responsivas e estilizadas, fornecendo um conjunto de estilos predefinidos e componentes reutilizáveis, agilizando o processo de criação de páginas web modernas e atraentes.</p></li>
  </li>
  <li><a href="https://www.figma.com/">Figma</a>: Figma é uma ferramenta de design colaborativo baseada na nuvem, que permite criar interfaces de usuário, protótipos interativos e compartilhar facilmente os designs com equipes de trabalho, agilizando o processo de design e feedback em projetos de design de produtos e interfaces digitais.</p></li>
  </li>

  </ul>
  
  <h2 style="font-family:roboto;"> Contribuições Individuais :dart:</h2>
  
  <h3> Atribuições como Desenvolvedor Front-end</h3>

Fui responsável por ajudar no desenvolvimento front-end da aplicação. Por ser o terceiro semestre do curso, já havia construído uma base de conhecimentos necessários para desenvolver o projeto, embora o uso de tecnologias diferentes das apresentadas anteriormente tenha dificultado o processo de desenvolvimento.
  
Sendo responsável pelo desenvolvimento do front-end do sistema, implementei serviços de cadastro, leitura e remoção de dados coletados pela aplicação. Também prestei apoio na criação das interfaces gráficas com o Java e no versionamento do projeto com a tecnologia Git.
  
</details>   

Participei de forma efetiva da integração do Front-End com Back-End, criando alguns métodos e realizando testes para validação das requisições.

 <details open><summary>Informações código Front-End</summary>
  
  
   1. Trecho do código responsável de receber o retorno do back-end, da explicação citada acima.
   
     
   ```js
   
        this.total = this.noDiscount += (element.price  * element.quantidade);

        this.service.getDiscount(this.id, this.quantidade, this.total, this.categoria).subscribe(
            response =>
            { const product : Product = new Product();
              this.discount = response;
              this.product.discount = this.discount
              this.finalPrice = this.finalPrice += (element.price * element.quantidade)-(this.discount)
              console.log("teste", this.categoria)
            errorResponse => console.log(errorResponse)
        })
    });
         
         ...
         
         return new ResponseEntity<>(desconto, HttpStatus.OK);     
   ```
   - Esse método é responsável por passar os parâmetros para o back-end, processar a informação e direcionar o retorno para a camada de visualização do usuário,
  sendo um trecho importante pois enviar dados, processa o retorno e já devolve os resultados para usuário.


Click aqui [GitHub](https://github.com/Doc-Docker/APIMidAll/blob/main/frontend-midall/src/app/cart.service.ts) para mais detalhes da implementação do método responsável por enviar a requisição para o back-end. 

</details>   

<br>

Implementação das telas de cadastro de produtos; </br>
   Desenvolvimento do formulário de cadastro de produtos, criação da classe de services para envio da requisição POST com objeto do tipo produto.
   
   <details>
      <summary>Código da função na classe service para criação e atualização de produtos </summary>
      
          onSubmit(){

           if(this.id){
             this.service.update(this.id, this.product)
             .subscribe( res => {
               this.success = true;
               this.errors = null;
             }
             )
           }
           else{

             this.service
               .insert(this.product)
               .subscribe( res =>{
                 this.success = true;
                 this.errors = null;

               }, errorRes =>{
                 this.success = false;
                 this.errors = errorRes.error.errors

               }

               )
           }


         }
   </details>
   
<br>
   
Implementação da interface do carrinho de compras;</br>
   Desenvolvimento de uma tela para mostrar todos os produtos selecionados pelo usuário no sistema
   <details>
      <summary>Código html para exibição dos produtos </summary>
      
 ```html
          <table class="table table-condensed table-hover">
                <thead>
                    <tr>
                        <th>Name</th>
                        <th>Price</th>
                        <th>Quantity</th>
                        <th>Discount</th>
                        <th></th>
                    </tr>
                </thead>
                <tbody>
                    <tr *ngFor="let p of products">
                        <td>{{ p.name }}</td>
                        <td>{{ p.price }}</td>
                        <td>{{ p.quantidade}}</td>
                        <td>-{{ p.discount }}</td>

                        <td>
                            <button  class="btn btn-warning" (click)="deleteProduct(p)">
                                <i class="fa fa-trash"></i>
                                Delete
                            </button>
                        </td>


                    </tr>
                </tbody>
                
            </table>
 ```
 
   </details>
  
Contudo, vale acrescentar que por ser o primeiro contato com uma empresa terceira no curso de Banco de Dados, o desafio foi diferente do projeto anterior pois deveríamos atender os requisitos necessários e ter uma comunicação ativa com o cliente a fim de produzir entregas de valores a cada etapa do processo, por isso ajudei a gerenciar a equipe utilizando a metodologia ágil Scrum.

<h2 style="font-family:roboto;"> Aprendizados Efetivos :book:</h2>  

A MidAll foi primeiro sistema web com o qual trabalhei. Em seu desenvolvimento, obtive meu primeiro contato com conceitos bases para todo profissional desenvolvedor de software.

A integração do projeto com as matérias do semestre se deu em diversas frentes. A mais importante delas foi na disciplina de Engenharia de Software. Durante o semestre de desenvolvimento deste trabalho, iniciamos o aprendizado sobre diversos padrões de projeto nesta disciplina, pela primeira vez. Com isso, pela primeira vez nos preocupamos em separar nosso programa que se tornaria o produto em camadas, seguir padrões de arquitetura, torná-lo componentizável e seguindo modos de construção comuns aos utilizados no mercado e comunidade. Foi o passo inicial de estudo sobre tais competências tão importantes para qualquer desenvolvedor de software.

Além destes itens importantes que foram citados acima, outros aprendizados importantes precisam ser mencionados:

Durante o desenvolvimento do projeto, a performance do sistema foi uma questão central em seu desenvolvimento.
Possuíamos uma base de dados minimamente volumosa, e precisávamos calcular diversos fatores de todos os seus registros. Com isso, precisávamos pensar em formas mais eficientes em processamento para garantir uma resposta rápida e confiável ao nosso usuário final. A evolução nos algoritmos de análise de dados com o passar do projeto é algo que foi de grande valia para a nossa formação como profissionais desenvolvedores.

  <h3 align="center"> Hard Skills </h3>
  <table align="center">
    <tr>
      <th width="300px">Tecnologia/Metodologia</th>
      <th width="300px">Classificação</th>
    </tr>
    <tr>
      <td>Metodologia Ágil Scrum</td>
      <td>★★★★☆</td>
    </tr>
    <tr>
      <td>Microsoft SQL Server</td>
      <td>★★★☆☆</td>
    </tr>	
    <tr>
      <td>Java</td>
      <td>★★☆☆☆</td>
    </tr>
    <tr>
      <td>Angular</td>
      <td>★★★☆☆</td>
    </tr>
   <tr>
      <td>CSS</td>
      <td>★★★★☆</td>
    </tr>
   <tr>
      <td>Bootstrap</td>
      <td>★★★★☆</td>
    </tr>
    <tr>
      <td>Figma</td>
      <td>★★★★☆</td>
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

   <p align="justify" style="font-family:roboto;"><li><a href="https://github.com/BryanRibeiro/Portfolio-Projetos/blob/main/API_1.md"> 1º Semestre: SOS EDUCA - Site de Vendas de Materiais Didáticos</a></li></p>
   <p align="justify" style="font-family:roboto;"><li><a href="https://github.com/BryanRibeiro/Portfolio-Projetos/blob/main/API_2.md">2º Semestre: GSW - Dashboard para acompanhamentos dos projetos, através de diferentes fontes de dados.</a></li></p>
   <p align="justify" style="font-family:roboto;"><li> 3° Semestre: PromoAll - Ecommerce com um motor de regras para promoções aplicadas no momento da compra.</a></li></p>
   <p align="justify" style="font-family:roboto;"><li><a href="https://github.com/BryanRibeiro/Portfolio-Projetos/blob/main/API_4.md">4° Semestre: Subiter - Aplicação Web para sincronização dos dados administrativos, financeiros e operacionais.</a></li></p>
   <p align="justify" style="font-family:roboto;"><li><a href="https://github.com/BryanRibeiro/Portfolio-Projetos/blob/main/API_5.md">5º Semestre: Em Construção 🏗️</a></li></p>
   <p align="justify" style="font-family:roboto;"><li><a href="https://github.com/BryanRibeiro/Portfolio-Projetos/blob/main/API_6.md">6º Semestre: Em Construção 🏗️</a></li></p>
  
</body>
</html>
