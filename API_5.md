<html>
<body>
 <h1 align="center"> API 5º Semestre - 01/2023</h1>
 <h1 align="center"> 
<a href="https://github.com/TechNinjass/midall-parent"><img src="https://img.shields.io/badge/GitHub-Repositório Projeto-181717?style=for-the-badge&logo=github"></a>
</h1>
 
 <h2> Parceiro Acadêmico: <a href="https://midall.com.br/">MidAll [B]</a></h2>
 
<img src="https://github.com/BryanRibeiro/Portfolio-Projetos/blob/main/images/logo%20midall.png" height="150" width="230"/>

  <h2 style="font-family:roboto;"> Resumo do Projeto :clipboard:</h2>
  
  <p align="justify" style="font-family:roboto;"> O projeto consiste na automação do processo de download de arquivos armazenados na nuvem, transferindo-os para outra nuvem. Isso é realizado por meio do desenvolvimento de uma aplicação como serviço, que oferece um menu de configuração simples para os usuários. Os parâmetros inseridos nesse menu são utilizados para automatizar o download dos arquivos, com a aplicação gerando alertas em caso de falhas no processamento. A aplicação é executada em um servidor local e conta com telas dedicadas à configuração do sistema e à definição dos dados de acesso à API. O sistema emite alertas no sistema operacional para informar sobre novos arquivos baixados e mantém um histórico desses downloads.

   Além disso, foi construída uma API que funciona como o serviço responsável por buscar os arquivos de forma automática, seguindo as configurações previamente definidas pelo usuário. Os metadados dos arquivos são salvos para a criação de um dashboard que permite monitorar a execução do serviço, analisar resultados e visualizar indicadores de desempenho.
  
<h2 style="font-family:roboto;"> Tecnologias Adotadas :computer:</h2>
 
 <div style="display: inline_block"><br> 
 <img src="https://github.com/devicons/devicon/blob/master/icons/microsoftsqlserver/microsoftsqlserver-plain-wordmark.svg" width="100"    height="100" />	 
 <img src="https://raw.githubusercontent.com/devicons/devicon/1119b9f84c0290e0f0b38982099a2bd027a48bf1/icons/python/python-original-wordmark.svg" width="100"    height="100" />
 <img src="https://raw.githubusercontent.com/devicons/devicon/1119b9f84c0290e0f0b38982099a2bd027a48bf1/icons/vuejs/vuejs-original.svg" width="100" height="100" />
 <img src="https://raw.githubusercontent.com/devicons/devicon/1119b9f84c0290e0f0b38982099a2bd027a48bf1/icons/html5/html5-original-wordmark.svg" width="100" height="100" />
 <img src="https://raw.githubusercontent.com/devicons/devicon/1119b9f84c0290e0f0b38982099a2bd027a48bf1/icons/javascript/javascript-original.svg" width="100" height="100" />
 <img src="https://raw.githubusercontent.com/devicons/devicon/1119b9f84c0290e0f0b38982099a2bd027a48bf1/icons/docker/docker-original-wordmark.svg" width="100" height="100" />
 <img src="https://raw.githubusercontent.com/devicons/devicon/1119b9f84c0290e0f0b38982099a2bd027a48bf1/icons/figma/figma-original.svg" width="100" height="100" />
</div>
 
<br>
 
  <ul>
  <li><a href="https://azure.microsoft.com/">Microsoft SQL Server</a>: O Microsoft SQL Server é um sistema de gerenciamento de banco de dados relacional desenvolvido pela Microsoft, amplamente utilizado para armazenar, manipular e recuperar dados de forma eficiente e segura.</p></li>
  </li>	  
  <li><a href="https://www.python.org/">Python</a>: Python é uma linguagem de programação de alto nível, interpretada e de propósito geral, conhecida por sua simplicidade, legibilidade e ampla aplicabilidade em diferentes domínios, desde desenvolvimento web até análise de dados.</p></li>
  </li>
   <li><a href="https://vuejs.org/">Vue.js</a>: O Vue.js é um framework JavaScript progressivo e de código aberto para construção de interfaces de usuário interativas e dinâmicas. Ele oferece uma abordagem simples e flexível para o desenvolvimento de aplicações web modernas.</p></li>
  </li>
  <li><a href="https://html.spec.whatwg.org/multipage/">HTML</a>: É uma linguagem de marcação utilizada para estruturar e organizar o conteúdo das páginas da web. Com suas tags e elementos, permite a criação de textos, imagens, links e formulários, fornecendo a base fundamental para a construção de sites. É complementado por outras tecnologias como CSS e JavaScript para estilização e interatividade.</p></li>
  </li>
   <li><a href="https://developer.mozilla.org/pt-BR/docs/Web/JavaScript">JavaScript</a>: É uma linguagem de programação versátil e poderosa, utilizada para adicionar interatividade, funcionalidades dinâmicas e comportamentos aos sites.</p></li>
  </li>
   <li><a href="https://www.docker.com/">Docker</a>: O Docker é uma plataforma de virtualização leve e portátil que permite empacotar, distribuir e executar aplicativos de forma isolada, garantindo a portabilidade e consistência do ambiente de desenvolvimento e produção.</p></li>
  </li>
  <li><a href="https://www.figma.com/">Figma</a>: Figma é uma ferramenta de design colaborativo baseada na nuvem, que permite criar interfaces de usuário, protótipos interativos e compartilhar facilmente os designs com equipes de trabalho, agilizando o processo de design e feedback em projetos de design de produtos e interfaces digitais.</p></li>
  </li>

  </ul>

  <h2 style="font-family:roboto;"> Contribuições Individuais :dart:</h2>
  
  <h3> Atribuições como Desenvolvedor Front-End</h3>

Implementei o código abaixo, criando uma funcionalidade de listagem de arquivos com histórico de transferência para o Amazon S3. Inicialmente, importei os componentes essenciais, como DataTable, Column e Cabecalho do PrimeVue, além do módulo ListagemArquivos, responsável por obter os dados da transferência.

Ao desenvolver o componente 'TabelaView' em Vue.js, utilizei o método listar para obter a lista de arquivos e formatei os metadados, como tamanho e data de modificação, para proporcionar uma apresentação mais legível e compreensível ao usuário.

A implementação dos métodos específicos, como formatarData para lidar com datas e converterSize para ajustar os tamanhos dos arquivos para megabytes, foi essencial para uma apresentação mais amigável das informações.

 <details>

<summary>Código em Vue.js - Tabela</summary>
 
 ```javascript
 
     <script>
    import DataTable from 'primevue/datatable';
    import Column from 'primevue/column';
    import ListagemArquivos from '../services/listagemArquivos';
    import Cabecalho from '../components/Cabecalho.vue';
    export default {
      name: 'TabelaView',
      
      components: {
        DataTable,
        Column,
        Cabecalho,
      },
      data() {
        return {
          dados: [],
          buscar_nome: "",
        };
      },
  
      mounted() {
        this.listar();
        this.formatacaoDados();
      },
      
      methods: {
        listar() {
          ListagemArquivos.listar().then((resposta) => {
            this.dados = resposta.data.files;
            resposta.data.files.forEach(item => {
              item.size = this.converterSize(item.size);
            });
          });
        },

        formatacaoDados() {
          this.converterTamanhoArquivos();
          this.converterData();
        },

        converterData() {
          this.dados.forEach(item => {
            item.LastModified = this.formatarData(item.LastModified);
          });
        },

        formatarData(data) {
          const date = new Date(data);
          const dia = date.getDate().toString().padStart(2, '0');
          const mes = (date.getMonth() + 1).toString().padStart(2, '0');
          const ano = date.getFullYear();
          return `${dia}/${mes}/${ano}`;
        },

        converterSize(size) {
          const sizeAtual = (size/1000);
          const sizeFinal = sizeAtual + "MB"
          return sizeFinal;
        },

        converterTamanhoArquivos() {
          this.dados.forEach(item => {
            item.size = this.converterSize(item.size);
          });
        },

        filtro() {
          this.novosDados = this.dados.filter(item => item.name.toLowerCase().includes(this.buscar_nome.toLowerCase()));
          this.dados = this.novosDados;
        },

        limpar() {
          this.buscar_nome = "";
          this.listar();
        },
      }
    };
  </script>
 
 ```
 
 </details> 

Enfrentei desafios ao integrar eficientemente o serviço AWS S3 para a obtenção dos dados. No entanto, a abordagem iterativa de desenvolvimento, testes e ajustes permitiu superar esses desafios com sucesso.

A funcionalidade de busca dinâmica foi implementada por meio do método filtro, garantindo que o usuário pudesse filtrar os arquivos com base no nome em tempo real. A inclusão do método limpar possibilitou reiniciar a busca e exibir todos os arquivos novamente, proporcionando uma experiência intuitiva ao usuário.

  <details>
     <summary>Clique aqui para visualizar a tela de listagem dos arquivos</summary>
     <br>
     <img style="border-radius: 50%; align: center" src="https://github.com/TechNinjass/midall-parent/blob/main/docs/Images/telalistagemarquivos.jpeg" width="1000px;" alt=""/>
  </details>

Em retrospectiva, a implementação deste componente não apenas atendeu ao requisito funcional de exibir o histórico de transferência de arquivos, mas também ressaltou a importância da abordagem cuidadosa na integração de serviços externos e na apresentação eficiente de dados na interface.

  <h3>Atribuições no uso de DevOps</h3>
    <p align="justify" style="font-family:roboto;"> O DevOps representa uma metodologia avançada de desenvolvimento de software que se fundamenta na comunicação eficaz entre desenvolvedores e profissionais de infraestrutura de TI, promovendo uma integração fluida entre os setores de desenvolvimento e operações. Seu principal propósito é acelerar e aprimorar a criação e gestão da infraestrutura de aplicações. Com uma abordagem centrada na cultura, automação e design de plataforma, busca incessantemente agregar valor aos negócios e ampliar a capacidade de resposta às mudanças, garantindo entregas de serviços rápidas e de alta qualidade.

Na prática, o DevOps engloba todo o ciclo de vida do software, desde o planejamento até a implementação, passando pela automação e prestação de serviços. Dessa forma, abarca integralmente cada etapa, contribuindo de maneira decisiva para alcançar o resultado final desejado.</p>
  <details>
     <summary>Clique aqui para visualizar os processos do DevOps</summary>
     <br>
     <img style="border-radius: 50%; align: center" src="https://github.com/BryanRibeiro/Portfolio-Projetos/blob/main/images/dev.png" width="400px;" alt=""/>
  </details>
  
 <p align="justify" style="font-family:roboto;"> A primeira prática no projeto foi a aplicação do Git Workflow. Abaixo, uma recomendação de como usar o Git e organizar suas branches para realizar um trabalho de maneira consistente e produtiva. A estrutura das branches para versionamento de código foi dividida da seguinte maneira:</p>
  <ul>
  <li> <p align="justify" style="font-family:roboto;">main - Concentra o código de produção, só pondendo ter mudanças por pull requests (permissão para alteração) da branch develop.</p>
  </li>
    
  <li> <p align="justify" style="font-family:roboto;">develop - Branch destinada para testes de funcionalidades e da ferramenta como um todo, só pode ter mudanças por meio de pull requests (permissão para alteração) das branches features.</p>
  </li>
    
  <li> <p align="justify" style="font-family:roboto;">features - Branches com objetivo de desenvolvimentos das funcionalidades do software.</p>
  </li>
  </ul>

### 🐳 Deploy no Docker

O Deploy é a prática de disponibilizar a aplicação para uso, seja em um ambiente de desenvolvimento, teste ou produção. O Docker é uma ferramenta que, por meio do uso de containers, facilita o deploy de uma aplicação. Com ela, é possível criar imagens que contêm tudo o que é necessário para o funcionamento da aplicação, como dependências e bibliotecas. Utilizar o Docker é uma maneira de fazer o deploy de uma aplicação em um servidor.

<details>
É uma ferramenta docker, usada para construir e configurar vários contêineres Docker simultaneamente. Você pode iniciar todos os seus serviços através de um arquivo de configuração (docker-compose.yml) com apenas um comando. Pode ser usado em todos os ambientes: produção, teste e desenvolvimento.
<br> <br>
<summary>Docker Compose</summary>

```java
version: "3"

services:
  backend-app:
    container_name: midall-backend-app
    image: midall-backend-app
    build:
      context: ../
      dockerfile: ./docker/flask.dockerfile
    restart: always
    ports:
      - "5000:5000"
    volumes:
      - ${FLASKR_BACK_DEV_DIR}:/flaskr
    env_file:
      - .env

networks:
  network:
    driver: bridge
    external: false
    name: midall-network

```
FLASKR_BACK_DEV_DIR é uma variável de ambiente definida no arquivo `.env`. Essa variável é o caminho onde está o volume da aplicação.

```java
FLASKR_BACK_DEV_DIR = project volume path
```

</details>


<details>
É um arquivo de configuração, como docker-compose.yml, usado para dar instruções durante a criação de containers. Podemos usá-lo para baixar arquivos, instalar pacotes e executar comandos shell.
<br> <br>
<summary>DockerFile</summary>

```java
FROM python:3.10.6-slim-buster

WORKDIR /flaskr/

COPY ./requirements.txt /flaskr/

WORKDIR /flaskr/

RUN pip install -r requirements.txt

CMD ["python", "-m", "flask", "run"]

```

</details>


<details>
É um arquivo que serve para excluir diretórios ou arquivos desnecessários no contexto de construção.
<br> <br>
<summary>DockerIgnore</summary>

```java
tests
.vscode
.coveragerc
.pytest.ini
*.iml
**/__pycache__
**/migrations/*
*.md
.git
.gitignore
!README*.md
README-secret.md

```

</details>

Neste projeto fizemos a documentação de cada item DevOps implementado. O link abaixo fornece uma descrição detalhada de cada item, explicando nosso fluxo de trabalho, metodologias utilizadas, ferramentas, tecnologias escolhidas e muito mais.

🔗 [Link da Documentação do DevOps no Wiki](https://github.com/TechNinjass/midall-parent/wiki)
  
  <h3> Atribuições como Product Owner</h3>
  <p align="justify" style="font-family:roboto;"> Como Product Owner nesse projeto desafiador, meu papel centralizou-se na orquestração do backlog de produto e na coordenação das tarefas do time de desenvolvimento, garantindo a conformidade com os objetivos estabelecidos. Trabalhei em estreita colaboração com as partes interessadas para compreender suas necessidades, enfrentando o desafio de traduzir essas demandas complexas em requisitos claros e priorizados.

O primeiro desafio enfrentado foi a compreensão abrangente dos requisitos de automação do processo de download, transferência e alertas em caso de falhas. Este processo demandou uma análise detalhada para identificar as funcionalidades cruciais e melhorias necessárias para superar os desafios do projeto. A organização e priorização das histórias de usuário foram realizadas considerando o valor agregado e o impacto nos resultados finais.

 <details>
      <summary>Backlogs, Epics & User Stories</summary>
<h1 align="center"> <img src = "https://github.com/TechNinjass/midall-parent/blob/main/docs/Images/documenta%C3%A7%C3%B5es-po.png" /></h1>
 
 </details> 
 
Tive que esclarecer dúvidas, fornecer orientações precisas e assegurar que todos estivessem alinhados com os objetivos do projeto foram elementos críticos. Conduzi reuniões de planejamento de sprint para revisão e refinamento do backlog, definindo metas para cada iteração. Colaborei ativamente com a equipe para segmentar as histórias de usuário em tarefas específicas e acionáveis, promovendo eficiência e compreensão clara das expectativas e prazos.</p>
 
<h2 style="font-family:roboto;"> Aprendizados Efetivos :book:</h2>  

Durante a implementação do projeto, adquiri aprendizados significativos que contribuíram para o meu desenvolvimento como desenvolvedor. A criação do componente 'TabelaView' para listar arquivos com histórico de transferência para o Amazon S3 proporcionou valiosas lições.

Ao adotar a abordagem DevOps, compreendi como a comunicação eficiente entre equipes pode acelerar o ciclo de desenvolvimento, otimizar a criação e gerenciamento da infraestrutura de aplicações, e promover entregas mais rápidas e de alta qualidade. Esse aprendizado não apenas aprimorou minha compreensão dos processos de desenvolvimento ágil, mas também enfatizou a importância da cultura, automação e design de plataforma no contexto do DevOps.

A introdução e aplicação do Docker no projeto foram fundamentais para facilitar o deployment da aplicação. Utilizando containers, pude criar imagens contendo todos os elementos necessários para o funcionamento da aplicação, simplificando o processo de transferência e garantindo consistência nos ambientes de desenvolvimento, teste e produção. Isso aprofundou meu conhecimento em virtualização e orquestração de contêineres, permitindo uma gestão eficiente da infraestrutura da aplicação.

  <h3 align="center"> Hard Skills </h3>
  <table align="center">
    <tr>
      <th width="300px">Tecnologia/Metodologia</th>
      <th width="300px">Classificação</th>
      <th width="300px">Escala de Aprendizado</th>
    </tr>
    <tr>
      <td>Metodologia Scrum - Product Owner</td>
      <td>★★★★★</td>
      <td>Sei fazer com autonomia</td>
    </tr>
    <tr>
      <td>Microsoft SQL Server</td>
      <td>★★★☆☆</td>
      <td>Entendi</td>
    </tr>	
    <tr>
      <td>Python</td>
      <td>★★★★☆</td>
      <td>Sei fazer com ajuda</td>
    </tr>
    <tr>
      <td>Vue.js</td>
      <td>★★★★☆</td>
      <td>Sei fazer com ajuda</td>
    </tr>
   <tr>
      <td>HTML</td>
      <td>★★★★★</td>
      <td>Sei fazer com autonomia</td>
    </tr>
   <tr>
      <td>JavaScript</td>
      <td>★★★★★</td>
      <td>Sei fazer com autonomia</td>
    </tr>
    <tr>
      <td>Docker</td>
      <td>★★★★☆</td>
      <td>Sei fazer com ajuda</td>
    </tr>
      <tr>
      <td>Figma</td>
      <td>★★★★★</td>
      <td>Sei fazer com autonomia</td>
    </tr>
  </table>
  
  <h3 align="center">Soft Skills</h3>
  <table align="center">
    <tr>
      <th width="300px">Habilidade</th>
      <th width="300px">Descrição</th>
    </tr>
<tr>
  <td>Aprendizado</td>
  <td>Adquiri um conhecimento maior ao assumir o papel de Product Owner pela segunda vez.</td>
</tr>
<tr>
  <td>Desenvolvimento de Equipe</td>
  <td>Trabalhei na melhoria da colaboração da equipe, utilizando práticas como Sprint Planning e Sprint Review.</td>
</tr>
<tr>
  <td>Feedback</td>
  <td>Aprimorei minhas habilidades de fornecer e receber feedback, contribuindo para a evolução contínua do produto.</td>
</tr>
<tr>
  <td>Gestão de Riscos</td>
  <td>Lidei com a identificação e mitigação de riscos, aplicando estratégias para garantir o sucesso do projeto.</td>
</tr>
<tr>
  <td>Adaptação</td>
  <td>Ajustei o planejamento do projeto conforme as mudanças nas necessidades do cliente, utilizando a abordagem ágil.</td>
</tr>
  </table>
  
---

 <h2 align="center"> Navegação Projetos :link:</h2>

   <p align="justify" style="font-family:roboto;"><li><a href="https://github.com/BryanRibeiro/Portfolio-Projetos/blob/main/API_1.md">1º Semestre: SOS EDUCA - Site de Vendas de Materiais Didáticos</a></li></p>
   <p align="justify" style="font-family:roboto;"><li><a href="https://github.com/BryanRibeiro/Portfolio-Projetos/blob/main/API_2.md">2º Semestre: GSW - Dashboard para acompanhamentos dos projetos, através de diferentes fontes de dados.</a></li></p>
   <p align="justify" style="font-family:roboto;"><li><a href="https://github.com/BryanRibeiro/Portfolio-Projetos/blob/main/API_3.md">3° Semestre: PromoAll - Ecommerce com um motor de regras para promoções aplicadas no momento da compra.</a></li></p>
   <p align="justify" style="font-family:roboto;"><li><a href="https://github.com/BryanRibeiro/Portfolio-Projetos/blob/main/API_4.md">4° Semestre: Subiter - Aplicação Web para sincronização dos dados administrativos, financeiros e operacionais.</a></li></p>
   <p align="justify" style="font-family:roboto;"><li>5º Semestre: Tech Ninjas - Automatização de transferência de arquivos entre nuvens.</a></li></p>
   <p align="justify" style="font-family:roboto;"><li><a href="https://github.com/BryanRibeiro/Portfolio-Projetos/blob/main/API_6.md">6º Semestre: Tech Vision - Sistema de Informação Geográfica de dados públicos do ProAgro.</a></li></p>
  
</body>
</html>






































