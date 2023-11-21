<html>
<body>
 <h1 align="center"> API 6º Semestre - 02/2023</h1>
 <h1 align="center"> 
<a href="https://github.com/TechVisionn/tech-parent"><img src="https://img.shields.io/badge/GitHub-Repositório Projeto-181717?style=for-the-badge&logo=github"></a>
</h1>
 
 <h2> Parceiro Acadêmico: <a href="https://visionaespacial.com/">Visiona Espacial</a></h2>
 
<img src="https://github.com/TechVisionn/tech-parent/blob/main/docs/Images/Logo_Visiona.png" height="130" width="300"/>

  <h2 style="font-family:roboto;"> Resumo do Projeto :clipboard:</h2>
  
  <p align="justify" style="font-family:roboto;"> O projeto visa a implementação de um Sistema de Informação Geográfica (SIG) para aprimorar a eficiência das análises e otimizar os processos internos. Embora os dados necessários estejam disponíveis no ProAgro, programa do governo federal destinado ao financiamento agrícola para pequenos e médios produtores brasileiros, a falta de organização, a presença de informações sensíveis e a sobrecarga de dados representam desafios significativos.

A proposta consiste em uma solução abrangente, que inclui a coleta e o refinamento dos dados públicos do ProAgro, a reestruturação eficiente da base de dados e o desenvolvimento de um SIG personalizado. Este sistema visa simplificar e organizar as informações, proporcionando aos usuários uma compreensão mais fácil e facilitando a análise dos dados. A proposta busca simplificar e organizar as informações, proporcionando aos usuários uma compreensão mais fácil e facilitando a análise dos dados. Destaca-se a organização do banco de dados público do ProAgro para permitir consultas e análises rápidas no Sistema de Informações Geográficas.
  
<h2 style="font-family:roboto;"> Tecnologias Adotadas :computer:</h2>
 
 <div style="display: inline_block"><br> 
 <img src="https://raw.githubusercontent.com/devicons/devicon/1119b9f84c0290e0f0b38982099a2bd027a48bf1/icons/mysql/mysql-original-wordmark.svg" width="100"    height="100" />	 
 <img src="https://github.com/TechVisionn/tech-parent/blob/main/docs/Images/Mongodb-PNG-Image-HD.png" width="100"    height="100" />
 <img src="https://raw.githubusercontent.com/devicons/devicon/1119b9f84c0290e0f0b38982099a2bd027a48bf1/icons/python/python-original-wordmark.svg" width="100"    height="100" />
 <img src="https://github.com/TechVisionn/tech-parent/blob/main/docs/Images/React-icon.svg.png" width="100" height="100" />
 <img src="https://raw.githubusercontent.com/devicons/devicon/1119b9f84c0290e0f0b38982099a2bd027a48bf1/icons/docker/docker-original-wordmark.svg" width="100" height="100" />
 <img src="https://github.com/TechVisionn/tech-parent/blob/main/docs/Images/github%20logo.png" width="100" height="100" />
</div>
 
<br>
 
  <ul>
  <li><a href="https://www.mysql.com/">MySQL</a>: É um sistema de gerenciamento de banco de dados (SGBD) relacional, ou seja, que utiliza a linguagem SQL como interface. Lançado sobre a licença GPL, possui como desenvolvedor a Oracle Corporation.</p></li>
  </li>	  
  <li><a href="https://www.mongodb.com/pt-br">MongoDB</a>: É um banco de dados NoSQL que armazena dados em documentos flexíveis usando um formato JSON. Ele oferece escalabilidade e flexibilidade para lidar com grandes volumes de dados e modelos de dados dinâmicos.</p></li>
  </li>
  <li><a href="https://www.python.org/">Python</a>: É uma linguagem de programação de alto nível, interpretada e de propósito geral, conhecida por sua simplicidade, legibilidade e ampla aplicabilidade em diferentes domínios, desde desenvolvimento web até análise de dados.</p></li>
  </li>
  <li><a href="https://react.dev/">React</a>: É uma biblioteca JavaScript para construir interfaces de usuário interativas e reativas. Desenvolvida pelo Facebook, permite a criação de componentes reutilizáveis para construir aplicativos web eficientes.</p></li>
  </li>
   <li><a href="https://www.docker.com/">Docker</a>: É uma plataforma de virtualização leve e portátil que permite empacotar, distribuir e executar aplicativos de forma isolada, garantindo a portabilidade e consistência do ambiente de desenvolvimento e produção.</p></li>
  </li>
  <li><a href="https://github.com/">GIT</a>: É uma ferramenta de design colaborativo baseada na nuvem, que permite criar interfaces de usuário, protótipos interativos e compartilhar facilmente os designs com equipes de trabalho, agilizando o processo de design e feedback em projetos de design de produtos e interfaces digitais.</p></li>
  </li>

  </ul>

  <h2 style="font-family:roboto;"> Contribuições Individuais :dart:</h2>
  
  <h3> Atribuições como Desenvolvedor Front-End</h3>

Implementei a configuração inicial do mapa e controles no componente Mapa do projeto. Primeiramente, personalizei o ícone padrão dos marcadores utilizando a biblioteca Leaflet. Isso foi feito através da definição de um novo ícone com uma imagem principal (icon) e uma sombra (iconShadow), sendo aplicado a todos os marcadores no mapa.

 <details>

<summary>Código em React - Configuração do Mapa</summary>
 
 ```jsx

import React, { Component } from "react";
import { MapContainer, TileLayer } from "react-leaflet";
import { SelectButton } from 'primereact/selectbutton';
import { Button } from "primereact/button";
import { Link } from "react-router-dom";
import L from "leaflet";
import { OpenStreetMapProvider, GeoSearchControl } from "leaflet-geosearch";
import "leaflet/dist/leaflet.css";
import "leaflet-geosearch/dist/geosearch.css";
import "leaflet-easyprint";
import 'primeicons/primeicons.css';
import icon from 'leaflet/dist/images/marker-icon.png';
import iconShadow from 'leaflet/dist/images/marker-shadow.png';
import { Chart } from "primereact/chart";

const DefaultIcon = L.icon({
  iconUrl: icon,
  shadowUrl: iconShadow,
});

L.Marker.prototype.options.icon = DefaultIcon;

const search = new GeoSearchControl({
  provider: new OpenStreetMapProvider({
    params: {
      countrycodes: 'BR',
    },
  }),
  autoComplete: true,
  style: 'bar',
  notFoundMessage: 'Endereço não encontrado!',
  searchLabel: 'Buscar endereço',
  showMarker: false,
  showPopup: false,
  autoClose: true
});

class Mapa extends Component {
  constructor(props) {
    // ... (Código do construtor)
  }

  componentDidMount() {
    // ... (Configuração de controles após o componente ser montado)
  }

  // ... (Métodos adicionais, como handleZoomChange, addCustomZoomResetControl, handleZoomReset, renderizarGlebas, toggleOption, etc.)

  render() {
    return (
      <div id="mapa">
        <MapContainer center={[-21, -49]} zoom={7} style={{ height: "100vh" }} ref={(ref) => (this.leafletMap = ref)}>
          <TileLayer url="https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png" />
          {this.state.plotarGlebas && this.renderizarGlebas()}
        </MapContainer>
        <div style={{ position: 'absolute', top: '10px', left: "93%", zIndex: 1000 }}>
          <Link to="/">
            <Button label="Sair" icon="pi pi-sign-out" severity="info" aria-label="Sair" />
          </Link>
        </div>
      </div>
    );
  }
}

export default Mapa;
 
 ```
 
 </details> 

Em seguida, configurei a barra de busca (GeoSearchControl) para permitir a busca de endereços no mapa. Utilizei a biblioteca Leaflet-Geosearch, especificando o provedor OpenStreetMap para pesquisa no Brasil (countrycodes: 'BR'). Personalizei o estilo da barra de busca como uma barra (style: 'bar') e configurei mensagens relacionadas à busca, como a mensagem exibida quando nenhum endereço é encontrado (notFoundMessage) e o rótulo da barra (searchLabel).

 <details>
  
<summary>Código em React - Impressão do Mapa</summary>
 
 ```jsx
 
const exportPrint = L.easyPrint({
  title: 'Imprimir Mapa',
  position: 'topleft',
  sizeModes: ['A4Landscape'],
  filename: 'mapa',
  exportOnly: true,
  hideControlContainer: true,
});

class Mapa extends Component {

  componentDidMount() {
    setTimeout(() => {
      this.leafletMap.addControl(search);
      this.leafletMap.addControl(exportPrint);  // Adição do controle de impressão ao mapa
      this.addCustomZoomResetControl();
      this.leafletMap.on('zoom', this.handleZoomChange);
      this.leafletMap.on('moveend', this.handleZoomChange);
    }, 100);
  }

  render() {
    return (
      <div id="mapa">
        <MapContainer center={[-21, -49]} zoom={7} style={{ height: "100vh" }} ref={(ref) => (this.leafletMap = ref)}>
          <TileLayer url="https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png" />
          {this.state.plotarGlebas && this.renderizarGlebas()}
        </MapContainer>
        <div style={{ position: 'absolute', top: '10px', left: "93%", zIndex: 1000 }}>
          <Link to="/">
            <Button label="Sair" icon="pi pi-sign-out" severity="info" aria-label="Sair" />
          </Link>
        </div>
      </div>
    );
  }
}

export default Mapa;
 
 ```
 
 </details> 

Além disso, integrei a funcionalidade de impressão do mapa (easyPrint) para permitir que os usuários imprimam o mapa de forma fácil e personalizada. Defini o título, posição e opções de exportação da impressão, como modos de tamanho de página e ocultação do contêiner de controle.

No componente Mapa, no método componentDidMount, adicionei os controles de busca e impressão ao mapa, bem como um controle personalizado para resetar o zoom. Também registrei manipuladores de eventos para detectar mudanças no zoom e movimentação do mapa, desencadeando a exibição das glebas quando o zoom atinge um nível específico.

 <details>

<summary>Código em React - Método Render</summary>
 
 ```jsx

render() {
  return (
    <div id="mapa">
      <MapContainer center={[-21, -49]} zoom={7} style={{ height: "100vh" }} ref={(ref) => (this.leafletMap = ref)}>
        <TileLayer url="https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png" />
        {this.state.plotarGlebas && this.renderizarGlebas()}
      </MapContainer>
      <div style={{ position: 'absolute', top: '10px', left: "93%", zIndex: 1000 }}>
        <Link to="/">
          <Button label="Sair" icon="pi pi-sign-out" severity="info" aria-label="Sair" />
        </Link>
      </div>
    </div>
  );
}
 
 ```
 
 </details> 

No método render, configurei a estrutura do mapa usando o componente MapContainer fornecido pelo React-Leaflet, adicionando uma camada de azulejos do OpenStreetMap. A renderização das glebas é condicional, ocorrendo apenas quando a variável de estado plotarGlebas é verdadeira. Adicionalmente, incluí um botão de saída no canto superior direito, permitindo ao usuário retornar à página principal.

Essas implementações visam criar uma experiência de usuário interativa e informativa ao explorar o mapa de glebas do ProAgro.
  
  <h3> Atribuições como Product Owner</h3>
  <p align="justify" style="font-family:roboto;"> Como Product Owner, assumi a responsabilidade de liderar a definição e priorização do backlog de produto, assegurando que as metas estivessem alinhadas com os objetivos estabelecidos. Colaborei estreitamente com as partes interessadas para compreender suas necessidades, traduzindo-as em requisitos claros e priorizados.

Conduzi uma análise detalhada dos desafios relacionados à organização dos dados provenientes do ProAgro, destacando a falta de estrutura e a sobrecarga de informações. Com base nessa análise, elaborei o backlog de produto, identificando funcionalidades cruciais para superar os obstáculos identificados. Priorizei as histórias de usuário considerando o valor agregado e o impacto nos resultados do projeto.

 <details>
      <summary>Clique aqui para visualizar os Backlogs</summary>
<h1 align="center"> <img src = "https://github.com/TechVisionn/tech-parent/blob/main/docs/Images/English%20Backlog.png" /></h1>
 
 </details> 
 
Durante o ciclo de desenvolvimento, mantive uma comunicação contínua com a equipe, esclarecendo dúvidas, fornecendo direcionamentos e garantindo a conformidade com os objetivos do projeto. Facilitei reuniões de planejamento de sprint para revisão e refinamento do backlog, colaborando na definição de metas para cada iteração. A abordagem permitiu uma execução mais eficiente, com um fluxo de trabalho contínuo e uma compreensão aprimorada das expectativas e prazos por parte da equipe de desenvolvimento.</p>
 
<h2 style="font-family:roboto;"> Aprendizados Efetivos :book:</h2>  

Durante a execução do projeto, enfrentei desafios significativos que contribuíram para meu aprendizado e crescimento profissional. Lidar com a falta de organização e a presença de informações sensíveis nos dados públicos do ProAgro exigiu habilidades avançadas de manipulação e refinamento de dados.

Ao reestruturar a base de dados de forma eficiente, pude aprimorar minhas habilidades em modelagem e organização de informações geográficas. A criação de um Sistema de Informação Geográfica (SIG) personalizado demandou compreensão aprofundada de tecnologias específicas e a capacidade de integrar dados de maneira coesa.

Além disso, destaco a importância de simplificar e organizar as informações para facilitar a compreensão e análise dos dados pelos usuários. Essa abordagem visou melhorar a usabilidade do sistema, proporcionando uma experiência mais intuitiva e eficiente.

Participar ativamente da organização do banco de dados público do ProAgro permitiu-me desenvolver estratégias para consultas e análises rápidas no contexto do SIG. Essa experiência não apenas aprimorou minhas habilidades técnicas, mas também me proporcionou uma compreensão mais profunda dos desafios enfrentados ao lidar com dados governamentais sensíveis.

No geral, o projeto me proporcionou uma oportunidade valiosa de aplicar meus conhecimentos em um contexto prático, contribuindo para o desenvolvimento de soluções eficientes e impactantes.

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
      <td>MySQL</td>
      <td>★★★★☆</td>
      <td>Sei fazer com ajuda</td>
    </tr>	
    <tr>
      <td>MongoDB</td>
      <td>★★★★☆</td>
      <td>Sei fazer com ajuda</td>
    </tr>
    <tr>
      <td>Python</td>
      <td>★★★★☆</td>
      <td>Sei fazer com ajuda</td>
    </tr>
   <tr>
      <td>React</td>
      <td>★★★★★</td>
      <td>Sei fazer com autonomia</td>
    </tr>
   <tr>
      <td>Docker</td>
      <td>★★★★☆</td>
      <td>Sei fazer com ajuda</td>
    </tr>
    <tr>
      <td>GIT</td>
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
  <td>Colaboração Interfuncional</td>
  <td>Fomentei a colaboração entre diferentes áreas, promovendo uma abordagem integrada na execução do projeto.</td>
</tr>
<tr>
  <td>Empatia com o Usuário</td>
  <td>Aprofundei minha compreensão das necessidades dos usuários, priorizando funcionalidades que agregam valor real.</td>
</tr>
<tr>
  <td>Estimativas e Métricas</td>
  <td>Refinei as habilidades de estimar prazos e medir o desempenho do time, utilizando métricas relevantes.</td>
</tr>
<tr>
  <td>Negociação</td>
  <td>Aprimorei minhas habilidades de negociação para alinhar expectativas do cliente com a capacidade da equipe.</td>
</tr>
<tr>
  <td>Otimização Contínua</td>
  <td>Implementei práticas de melhoria contínua, analisando retrospectivas para aprimorar o processo de desenvolvimento.</td>
</tr>
  </table>
  
---

 <h2 align="center"> Navegação Projetos :link:</h2>

   <p align="justify" style="font-family:roboto;"><li><a href="https://github.com/BryanRibeiro/Portfolio-Projetos/blob/main/API_1.md">1º Semestre: SOS EDUCA - Site de Vendas de Materiais Didáticos.</a></li></p>
   <p align="justify" style="font-family:roboto;"><li><a href="https://github.com/BryanRibeiro/Portfolio-Projetos/blob/main/API_2.md">2º Semestre: GSW - Dashboard para acompanhamento dos projetos, através de diferentes fontes de dados.</a></li></p>
   <p align="justify" style="font-family:roboto;"><li><a href="https://github.com/BryanRibeiro/Portfolio-Projetos/blob/main/API_3.md">3° Semestre: PromoAll - Ecommerce com um motor de regras para promoções aplicadas no momento da compra.</a></li></p>
   <p align="justify" style="font-family:roboto;"><li><a href="https://github.com/BryanRibeiro/Portfolio-Projetos/blob/main/API_4.md">4° Semestre: Subiter - Aplicação Web para sincronização dos dados administrativos, financeiros e operacionais.</a></li></p>
   <p align="justify" style="font-family:roboto;"><li><a href="https://github.com/BryanRibeiro/Portfolio-Projetos/blob/main/API_5.md">5º Semestre: Tech Ninjas - Automatização de transferência de arquivos entre nuvens.</a></li></p>
   <p align="justify" style="font-family:roboto;"><li>6º Semestre: Tech Vision - Sistema de Informação Geográfica de dados públicos do ProAgro.</a></li></p>
  
</body>
</html>
