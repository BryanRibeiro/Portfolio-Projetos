<html>
<body>
 <h1 align="center"> API 4º Semestre - 02/2022</h1>
<a href="https://github.com/Doc-Docker/APISubiter"><img src="https://img.shields.io/badge/GitHub-Repositório Projeto-181717?style=for-the-badge&logo=github"></a>
 
 <h2> Parceiro Acadêmico: <a href="https://www.subiter.com/">Subiter</a></h2>
 
<img src="https://github.com/BryanRibeiro/Portfolio-Projetos/blob/main/images/logosubiter.png" height="150" width="250"/>
  
  <h2 style="font-family:roboto;"> Resumo do Projeto :clipboard:</h2>
  
  <p align="justify" style="font-family:roboto;"> O projeto tinha como objetivo solucionar o desafio de sincronização dos dados administrativos, financeiros e operacionais relacionados aos serviços prestados pela empresa. Na época, a falta de organização desses dados resultava em lentidão para atender chamados e dificuldades na interpretação dos indicadores comerciais e financeiros.

Para resolver essa questão, foi necessário implementar um sistema de gerenciamento integrado que centralizasse e organizasse todas as informações relevantes. Isso envolveu a criação de um banco de dados robusto e escalável, capaz de armazenar e gerenciar dados de diferentes áreas da empresa, como atendimento ao cliente, vendas, finanças e operações.

A implementação do sistema de gerenciamento integrado proporcionou vários benefícios. Em primeiro lugar, a sincronização dos dados permitiu um atendimento mais ágil aos chamados, pois as informações ficaram disponíveis de forma organizada e de fácil acesso para os colaboradores responsáveis por resolver os problemas dos clientes.

Além disso, a centralização dos dados administrativos, financeiros e operacionais possibilitou uma análise mais precisa dos indicadores comerciais e financeiros da empresa. Foi possível gerar relatórios e métricas atualizados em tempo real, facilitando a interpretação dos dados e auxiliando na tomada de decisões estratégicas.

<h2 style="font-family:roboto;"> Tecnologias Adotadas :computer:</h2>
 
 <div style="display: inline_block"><br> 
 <img src="https://raw.githubusercontent.com/devicons/devicon/1119b9f84c0290e0f0b38982099a2bd027a48bf1/icons/oracle/oracle-original.svg" width="100"    height="100" />	 
 <img src="https://raw.githubusercontent.com/devicons/devicon/1119b9f84c0290e0f0b38982099a2bd027a48bf1/icons/java/java-original-wordmark.svg" width="100"    height="100" />
 <img src="https://raw.githubusercontent.com/devicons/devicon/1119b9f84c0290e0f0b38982099a2bd027a48bf1/icons/vuejs/vuejs-original.svg" width="100" height="100" />
 <img src="https://raw.githubusercontent.com/devicons/devicon/1119b9f84c0290e0f0b38982099a2bd027a48bf1/icons/docker/docker-original-wordmark.svg" width="100" height="100" />
 <img src="https://raw.githubusercontent.com/devicons/devicon/1119b9f84c0290e0f0b38982099a2bd027a48bf1/icons/bootstrap/bootstrap-original-wordmark.svg" width="100" height="100" />
 <img src="https://raw.githubusercontent.com/devicons/devicon/1119b9f84c0290e0f0b38982099a2bd027a48bf1/icons/intellij/intellij-original.svg" width="100" height="100" />
</div>
 
<br>
 
  <ul>
  <li><a href="https://www.oracle.com/br/cloud/">Oracle Cloud</a>: A Oracle Cloud é uma plataforma de nuvem que oferece serviços abrangentes de armazenamento, computação e aplicativos, além de ser altamente escalável e segura.</p></li>
  </li>	  
  <li><a href="https://www.java.com/pt-BR/">Java</a>: Java é uma linguagem de programação de alto nível, multiplataforma e orientada a objetos, conhecida por sua portabilidade e segurança, amplamente usada no desenvolvimento de aplicativos e sistemas corporativos.</p></li>
  </li>
   <li><a href="https://vuejs.org/">Vue.js</a>: O Vue.js é um framework JavaScript progressivo e de código aberto para construção de interfaces de usuário interativas e dinâmicas. Ele oferece uma abordagem simples e flexível para o desenvolvimento de aplicações web modernas.</p></li>
  </li>
   <li><a href="https://www.docker.com/">Docker</a>: O Docker é uma plataforma de virtualização leve e portátil que permite empacotar, distribuir e executar aplicativos de forma isolada, garantindo a portabilidade e consistência do ambiente de desenvolvimento e produção.</p></li>
  </li>
   <li><a href="https://getbootstrap.com/">Bootstrap</a>: Bootstrap é um framework front-end de código aberto que facilita o desenvolvimento de interfaces responsivas e estilizadas, fornecendo um conjunto de estilos predefinidos e componentes reutilizáveis, agilizando o processo de criação de páginas web modernas e atraentes.</p></li>
  </li>
  <li><a href="https://www.jetbrains.com/idea/">IntelliJ IDEA</a>: O IntelliJ IDEA é um ambiente de desenvolvimento integrado (IDE) altamente produtivo para programação em diversas linguagens.</p></li>
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

Neste projeto pude aprimorar minha habilidade em trabalhar com o Oracle Cloud como banco de dados, adquirindo conhecimentos específicos dessa tecnologia. Também tive a oportunidade de aprofundar meus conhecimentos em Java e Spring Boot, utilizando essas ferramentas para implementar a lógica do back-end do sistema.

No front-end, desenvolvi minhas habilidades em HTML, JavaScript com Vue.js, CSS e Bootstrap, permitindo criar interfaces interativas e responsivas para o sistema de gerenciamento integrado. A combinação dessas tecnologias proporcionou uma experiência de usuário mais intuitiva e amigável.

Além disso, o projeto me ensinou a importância da organização e centralização dos dados, assim como a sincronização e integração de informações entre diferentes áreas de uma empresa. Compreendi a relevância de ter um sistema capaz de disponibilizar os dados de forma rápida e organizada, permitindo melhorias significativas no atendimento ao cliente e na análise dos indicadores comerciais e financeiros.

  <h3 align="center"> Hard Skills </h3>
  <table align="center">
    <tr>
      <th width="300px">Tecnologia/Metodologia</th>
      <th width="300px">Classificação</th>
    </tr>
    <tr>
      <td>Metodologia Scrum - Product Owner</td>
      <td>★★★★☆</td>
    </tr>
    <tr>
      <td>Oracle Cloud</td>
      <td>★★★☆☆</td>
    </tr>	
    <tr>
      <td>Java</td>
      <td>★★★☆☆</td>
    </tr>
    <tr>
      <td>Vue.js</td>
      <td>★★★☆☆</td>
    </tr>
   <tr>
      <td>Docker</td>
      <td>★★★★☆</td>
    </tr>
   <tr>
      <td>Bootstrap</td>
      <td>★★★★★</td>
    </tr>
    <tr>
      <td>IntelliJ IDEA</td>
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
      <td>Responsabilidade</td>
      <td>Assumi o cargo de Product Owner pela primeira vez.</td>
    </tr>
    <tr>
      <td>Visão de Negócio</td>
      <td>Compreendi melhor os problemas e expectativas do cliente, aplicando o Product Backlog Building.</td>
    </tr>
    <tr>
      <td>Comunicação</td>
      <td>Precisei me comunicar com o cliente com resiliência, e transmitir os requisitos para equipe dev.</td>
    </tr>
    <tr>
      <td>Organização</td>
      <td>Precisei organizar as tarefas do time e definir as prioridades.</td>
    </tr>
    <tr>
      <td>Planejamento</td>
      <td>Precisei planejar o escopo do projeto e construir o Product Backlog de uma forma prática.</td>
    </tr>
  </table>
  
---

 <h2 align="center"> Navegação Projetos :link:</h2>

   <p align="justify" style="font-family:roboto;"><li><a href="https://github.com/BryanRibeiro/Portfolio-Projetos/blob/main/API_1.md">1º Semestre: SOS EDUCA - Site de Vendas de Materiais Didáticos</a></li></p>
   <p align="justify" style="font-family:roboto;"><li><a href="https://github.com/BryanRibeiro/Portfolio-Projetos/blob/main/API_2.md">2º Semestre: GSW - Dashboard para acompanhamentos dos projetos, através de diferentes fontes de dados.</a></li></p>
   <p align="justify" style="font-family:roboto;"><li><a href="https://github.com/BryanRibeiro/Portfolio-Projetos/blob/main/API_3.md">3° Semestre: PromoAll - Ecommerce com um motor de regras para promoções aplicadas no momento da compra.</a></li></p>
   <p align="justify" style="font-family:roboto;"><li>4° Semestre: Subiter - Aplicação Web para sincronização dos dados administrativos, financeiros e operacionais.</a></li></p>
   <p align="justify" style="font-family:roboto;"><li><a href="https://github.com/BryanRibeiro/Portfolio-Projetos/blob/main/API_5.md">5º Semestre: Em Construção 🏗️</a></li></p>
   <p align="justify" style="font-family:roboto;"><li><a href="https://github.com/BryanRibeiro/Portfolio-Projetos/blob/main/API_6.md">6º Semestre: Em Construção 🏗️</a></li></p>
  
</body>
</html>
