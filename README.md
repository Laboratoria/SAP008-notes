# Lab Notes

## Índice

* [1. Prefácio](#1-prefácio)
* [2. Resumo do projeto](#2-resumo-do-projeto)
* [3. Objetivos de aprendizagem](#3-objetivos-de-aprendizagem)
* [4. Considerações gerais](#4-considerações-gerais)
* [5. Critérios de aceitação mínimos do projeto](#5-criterios-de-aceitação-mínimos-do-projeto)
* [6. Considerações técnicas](#6-considerações-técnicas)
* [7. Hacker edition](#7-hacker-edition)
* [8. Guias, dicas e leituras complementares](#8-guias-dicas-e-leituras-complementares)
***

## 1. Prefácio

[React](https://reactjs.org/), [Angular](https://angular.io/) e
[Vue](https://vuejs.org/) são alguns dos _frameworks_ e _bibliotecas_ de
JavaScript mais usados na área de desenvolvimento ao redor do mundo e existe uma
razão para isso. No contexto do navegador, [_manter a interface sincronizada com
o estado é
difícil_](https://medium.com/dailyjs/the-deepest-reason-why-modern-javascript-frameworks-exist-933b86ebc445).
Ao eleger um _framework_ ou _biblioteca_ para nossa interface, nos apoiamos em
uma série de convenções e implementações _testadas_ e _documentadas_ para
resolver um problema comum a toda interface web. Isto nos permite concentrar
melhor (dedicar mais tempo) nas características _específicas_ de nossa
aplicação.

Quando escolhemos uma destas tecnologias não só importamos um pedaço de código
para reusar (o qual já é um grande valor por si só), mas também adotamos uma
**arquitetura**, uma série de **princípios de design**, um paradigma, algumas
**abstrações**, um **vocabulário**, uma **comunidade**, etc...

Como desenvolvedora Front-End, estes kits de desenvolvimento podem resultar em
uma grande ajuda para implementar rapidamente _features_ dos projetos em que
você for trabalhar.

## 2. Resumo do projeto

Neste projeto construiremos uma aplicação para tomar notas, que nos permita
criar, editar, eliminar e consulta-las em qualquer momento.

Não existe dia em que não tomemos notas, sempre necessitamos guardar alguma
localização, número de telefone, notas de alguma reunião ou salvar nossas URLs
favoritas para consultar mais tarde. Muitas vezes para esta atividade
utilizamos cadernos ou agendas que acabam sendo esquecidas, ou anotamos de
manera dispersa de tal manera que perdemos de vista a prioridade e o propósito
da nota, no que resulta em uma nota perdida.

![Shows CRUD functionalities](https://raw.githubusercontent.com/florenciasilva/lab-notes/master/demo-crud.gif?token=AGJBHNTVAQRWOVF2IGMP6FK5NVFAS)

O objetivo principal é aprender a construir uma _interface web_ usando o
_framework_ escolhido (React). Esses framework front-end ataca
o seguinte problema: **como manter a interface e estado sincronizados**.
Portanto, esta experiência espera familiarizá-la com o conceito de _estado da
tela_, e como cada mudança no estado vai refletir na interface (por exemplo,
cada vez que adicionamos uma _nota_, a interface deve
atualizar a lista notas).

## 3. Objetivos de aprendizagem

Reflita e depois enumere os objetivos que quer alcançar e aplique no seu projeto. Pense nisso para decidir sua estratégia de trabalho.

### HTML

- [ ] **Uso de HTML semântico**

  <details><summary>Links</summary><p>

  * [HTML semântico](https://curriculum.laboratoria.la/pt/topics/html/02-html5/02-semantic-html)
  * [Semantics in HTML - MDN](https://developer.mozilla.org/en-US/docs/Glossary/Semantics#Semantics_in_HTML)
</p></details>

### CSS

- [ ] **Uso de seletores de CSS**

  <details><summary>Links</summary><p>

  * [Intro a CSS](https://curriculum.laboratoria.la/pt/topics/css/01-css/01-intro-css)
  * [CSS Selectors - MDN](https://developer.mozilla.org/pt_BR/docs/Web/CSS/CSS_Selectors)
</p></details>

- [ ] **Modelo de caixa (box model): borda, margem, preenchimento**

  <details><summary>Links</summary><p>

  * [Modelo de Caixa e Display](https://curriculum.laboratoria.la/pt/topics/css/01-css/02-boxmodel-and-display)
  * [The box model - MDN](https://developer.mozilla.org/en-US/docs/Learn/CSS/Building_blocks/The_box_model)
  * [Introduction to the CSS box model - MDN](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Box_Model/Introduction_to_the_CSS_box_model)
  * [CSS display - MDN](https://developer.mozilla.org/pt-BR/docs/Web/CSS/display)
  * [display - CSS Tricks](https://css-tricks.com/almanac/properties/d/display/)
</p></details>

- [ ] **Uso de flexbox em CSS**

  <details><summary>Links</summary><p>

  * [A Complete Guide to Flexbox - CSS Tricks](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)
  * [Flexbox Froggy](https://flexboxfroggy.com/#pt-br)
  * [Flexbox - MDN](https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Flexbox)
</p></details>

- [ ] **Uso de CSS Grid Layout**

  <details><summary>Links</summary><p>

  * [A Complete Guide to Grid - CSS Tricks](https://css-tricks.com/snippets/css/complete-guide-grid/)
  * [Grids - MDN](https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Grids)
</p></details>

- [ ] **Uso de media queries**

  <details><summary>Links</summary><p>

  * [CSS media queries - MDN](https://developer.mozilla.org/pt-BR/docs/Web/CSS/Media_Queries/Using_media_queries)
</p></details>

### JavaScript

- [ ] **Arrays (arranjos)**

  <details><summary>Links</summary><p>

  * [Arranjos](https://curriculum.laboratoria.la/pt/topics/javascript/04-arrays)
  * [Array - MDN](https://developer.mozilla.org//pt-BR/docs/Web/JavaScript/Reference/Global_Objects/Array/)
  * [Array.prototype.sort() - MDN](https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Reference/Global_Objects/Array/sort)
  * [Array.prototype.forEach() - MDN](https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Reference/Global_Objects/Array/forEach)
  * [Array.prototype.map() - MDN](https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Reference/Global_Objects/Array/map)
  * [Array.prototype.filter() - MDN](https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Reference/Global_Objects/Array/filter)
  * [Array.prototype.reduce() - MDN](https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Reference/Global_Objects/Array/Reduce)
</p></details>

- [ ] **Objetos (key, value)**

  <details><summary>Links</summary><p>

  * [Objetos em JavaScript](https://curriculum.laboratoria.la/pt/topics/javascript/05-objects/01-objects)
</p></details>

- [ ] **Diferenciar entre tipos de dados primitivos e não primitivos**

- [ ] **Uso de condicionais (if-else, switch, operador ternário, lógica booleana)**

  <details><summary>Links</summary><p>

  * [Estruturas condicionais e repetitivas](https://curriculum.laboratoria.la/pt/topics/javascript/02-flow-control/01-conditionals-and-loops)
  * [Tomando decisões no seu código — condicionais - MDN](https://developer.mozilla.org/pt-BR/docs/Learn/JavaScript/Building_blocks/conditionals)
</p></details>

- [ ] **Funções (params, args, return)**

  <details><summary>Links</summary><p>

  * [Funções (controle de fluxo)](https://curriculum.laboratoria.la/pt/topics/javascript/02-flow-control/03-functions)
  * [Funções clássicas](https://curriculum.laboratoria.la/pt/topics/javascript/03-functions/01-classic)
  * [Arrow Functions](https://curriculum.laboratoria.la/pt/topics/javascript/03-functions/02-arrow)
  * [Funções — blocos reutilizáveis de código - MDN](https://developer.mozilla.org/pt-BR/docs/Learn/JavaScript/Building_blocks/Functions)
</p></details>

- [ ] **Testes unitários (unit tests)**

  <details><summary>Links</summary><p>

  * [Introdução ao Jest - Documentação oficial](https://jestjs.io/docs/pt-BR/getting-started)
</p></details>

- [ ] **Testes assíncronos**

  <details><summary>Links</summary><p>

  * [Testando Código Assíncrono - Documentação oficial](https://jestjs.io/docs/pt-BR/asynchronous)
</p></details>

- [ ] **Uso de mocks e espiões**

  <details><summary>Links</summary><p>

  * [Simulações Manuais - Documentação oficial](https://jestjs.io/docs/pt-BR/manual-mocks)
</p></details>

- [ ] **Uso de linter (ESLINT)**

- [ ] **Uso de identificadores descritivos (Nomenclatura e Semântica)**

- [ ] **Diferença entre expressões (expressions) e declarações (statements)**

### Controle de Versões (Git e GitHub)

- [ ] **Git: Instalação e configuração**

- [ ] **Git: Controle de versão com git (init, clone, add, commit, status, push, pull, remote)**

- [ ] **Git: Integração de mudanças entre ramos (branch, checkout, fetch, merge, reset, rebase, tag)**

- [ ] **GitHub: Criação de contas e repositórios, configuração de chave SSH**

- [ ] **GitHub: Implantação com GitHub Pages**

  <details><summary>Links</summary><p>

  * [Site oficial do GitHub Pages](https://pages.github.com/)
</p></details>

### user-centricity

- [ ] **Desenhar e desenvolver um produto ou serviço colocando as usuárias no centro**

### product-design

- [ ] **Criar protótipos para obter feedback e iterar**

- [ ] **Aplicar os princípios de desenho visual (contraste, alinhamento, hierarquia)**

### Firebase

- [ ] **Firebase Auth**

  <details><summary>Links</summary><p>

  * [Primeiros passos com o Firebase Authentication em sites - Documentação oficial](https://firebase.google.com/docs/auth/web/start?hl=pt-BR)
  * [Gerenciar usuários no Firebase (onAuthStateChanged) - Documentação oficial](https://firebase.google.com/docs/auth/web/manage-users?hl=pt-BR)
</p></details>

- [ ] **Firestore**

  <details><summary>Links</summary><p>

  * [Firestore - Documentação oficial](https://firebase.google.com/docs/firestore?hl=pt-BR)
  * [Regras de segurança do Firebase - Documentação oficial](https://firebase.google.com/docs/rules?hl=pt-BR)
  * [Receber atualizações em tempo real com o Cloud Firestore - Documentação oficial](https://firebase.google.com/docs/firestore/query-data/listen?hl=pt-BR)
</p></details>

### Angular

- [ ] **Components & templates**

  <details><summary>Links</summary><p>

  * [Angular Components Overview - Documentação oficial (em inglês)](https://angular.io/guide/component-overview)
  * [Introduction to components and templates - Documentação oficial (em inglês)](https://angular.io/guide/architecture-components#introduction-to-components)
</p></details>

- [ ] **Diretivas estruturais (ngIf / ngFor)**

  <details><summary>Links</summary><p>

  * [Writing structural directives - Documentação oficial (em inglês)](https://angular.io/guide/structural-directives)
</p></details>

- [ ] **@Input | @Output**

  <details><summary>Links</summary><p>

  * [Component interaction - Documentação oficial (em inglês)](https://angular.io/guide/component-interaction#component-interaction)
</p></details>

- [ ] **Criação e uso de serviços**

  <details><summary>Links</summary><p>

  * [Providing services - Documentação oficial (em inglês)](https://angular.io/guide/architecture-services#providing-services)
</p></details>

- [ ] **Gerenciamento de rotas**

  <details><summary>Links</summary><p>

  * [In-app navigation: routing to views - Documentação oficial (em inglês)](https://angular.io/guide/router)
</p></details>

- [ ] **Criação e uso de Observables**

  <details><summary>Links</summary><p>

  * [Observables in Angular - Documentação oficial (em inglês)](https://angular.io/guide/observables-in-angular)
</p></details>

- [ ] **Uso de HttpClient**

  <details><summary>Links</summary><p>

  * [Communicating with backend services using HTTP - Documentação oficial (em inglês)](https://angular.io/guide/http)
</p></details>

- [ ] **Estilos de componentes (ngStyle / ngClass)**

  <details><summary>Links</summary><p>

  * [Template syntax - Documentação oficial (em inglês)](https://angular.io/guide/template-syntax#built-in-directives)
</p></details>

### React

- [ ] **JSX**

  <details><summary>Links</summary><p>

  * [Introduzindo JSX - Documentação oficial](https://pt-br.reactjs.org/docs/introducing-jsx.html)
</p></details>

- [ ] **Componentes e propriedades (props)**

  <details><summary>Links</summary><p>

  * [Componentes e propriedades - Documentação oficial](https://pt-br.reactjs.org/docs/components-and-props.html)
</p></details>

- [ ] **Manipulação de eventos**

  <details><summary>Links</summary><p>

  * [Manipulando eventos - Documentação oficial](https://pt-br.reactjs.org/docs/handling-events.html)
</p></details>

- [ ] **Listas e keys**

  <details><summary>Links</summary><p>

  * [Listas e chaves - Documentação oficial](https://pt-br.reactjs.org/docs/lists-and-keys.html)
</p></details>

- [ ] **Renderização condicional**

  <details><summary>Links</summary><p>

  * [Renderização condicional - Documentação oficial](https://pt-br.reactjs.org/docs/conditional-rendering.html)
</p></details>

- [ ] **Elevação de estado**

  <details><summary>Links</summary><p>

  * [Elevação de estado - Documentação oficial](https://pt-br.reactjs.org/docs/lifting-state-up.html)
</p></details>

- [ ] **Hooks**

  <details><summary>Links</summary><p>

  * [Introduzindo Hooks - Documentação oficial](https://pt-br.reactjs.org/docs/hooks-intro.html)
</p></details>

- [ ] **CSS modules**

  <details><summary>Links</summary><p>

  * [Adding a CSS Modules Stylesheet - Documentação de Create React App (em inglês)](https://create-react-app.dev/docs/adding-a-css-modules-stylesheet/)
</p></details>

- [ ] **React Router**

  <details><summary>Links</summary><p>

  * [Quick Start - Documentação oficial (em inglês)](https://reactrouter.com/web/guides/quick-start)
</p></details>

### Vue

- [ ] **Instância de Vue.js**

  <details><summary>Links</summary><p>

  * [A Instância Vue - Documentação oficial](https://br.vuejs.org/v2/guide/instance.html)
</p></details>

- [ ] **Dados e métodos**

  <details><summary>Links</summary><p>

  * [Dados e métodos - Documentação oficial](https://br.vuejs.org/v2/guide/instance.html#Dados-e-Metodos)
</p></details>

- [ ] **Uso e criação de componentes**

  <details><summary>Links</summary><p>

  * [Conceitos Básicos de Componentes - Documentação oficial](https://br.vuejs.org/v2/guide/components.html)
</p></details>

- [ ] **Props**

  <details><summary>Links</summary><p>

  * [Passando dados aos componentes filhos com Props - Documentação oficial](https://br.vuejs.org/v2/guide/components.html#Passando-Dados-aos-Filhos-com-Props)
</p></details>

- [ ] **Diretivas (v-bind | v-model)**

  <details><summary>Links</summary><p>

  * [v-bind - Documentação oficial](https://br.vuejs.org/v2/api/#v-bind)
  * [Binding/Interligações em Formulários - Documentação oficial](https://br.vuejs.org/v2/guide/forms.html)
</p></details>

- [ ] **Iteração (v-for)**

  <details><summary>Links</summary><p>

  * [Array em elementos com v-for - Documentação oficial](https://br.vuejs.org/v2/guide/list.html#Array-em-Elementos-com-v-for)
</p></details>

- [ ] **Eventos (v-on)**

  <details><summary>Links</summary><p>

  * [Manipulação de eventos - Documentação oficial](https://br.vuejs.org/v2/guide/events.html)
</p></details>

- [ ] **Dados Computados e Observadores**

  <details><summary>Links</summary><p>

  * [Dados Computados e Observadores](https://br.vuejs.org/v2/guide/computed.html)
</p></details>

- [ ] **Routing**

  <details><summary>Links</summary><p>

  * [Getting Started - Documentação oficial de Vue Router](https://router.vuejs.org/guide/#html)
</p></details>

- [ ] **Classes e Estilos**

  <details><summary>Links</summary><p>

  * [Interligações de Classe e Estilo - Documentação oficial](https://br.vuejs.org/v2/guide/class-and-style.html)
</p></details>

## 4. Considerações gerais

* Este projeto deve ser feito de forma individual.

* A duração estimada do projeto é de 4 sprints, com a duração de uma
  semana cada uma.

* Trabalhe integralmente uma história de usuário antes de passar para a próxima.

* O aplicativo deve ser um _Single Page App_. Os pedidos serão enviados por meio
de um _tablet_, mas **não queremos um aplicativo nativo**, mas sim um aplicativo
Web que seja **responsivo** e possa funcionar **offline**.

* Necessitamos pensar bem no aspecto UX de quem vai tomar as notas, o
tamanho e aspecto dos botões, a visibilidade do estado atual da nota,
etc.

* Implementar testes unitários dos componentes.

## 5. Critérios mínimos de aceitação do projeto

### Definição do produto

O [_Product Owner_](https://www.youtube.com/watch?v=7lhnYbmovb4) nos apresentou
este _backlog_ que é o resultado do seu trabalho colaborativo

***

### Histórias de usuário

#### [História de usuário 1] Usuário deve poder criar conta, iniciar e encerrar a sessão

Eu como usuária quero poder criar uma conta e entrar no sistema usando login pelo
Google para acessar minhas anotações.

***

#### [História de usuário 2] Usuário deve poder tomar nota

Eu como usuária quero tomar nota para não depender de minha
memória e ter acesso as anotações em todo momento, das coisas importantes que
antes escrevia no papel.

***

#### [História de usuário 3] Usuário deve poder ver as notas

Eu como usuária quero ler todas as notas para lembrar do que escrevi
antes.

***

#### [História de usuário 4] Usuário deve poder editar as notas

Eu como usuária quero editar as notas para  modificar o que
escrevi antes.

***

#### [História de usuário 5] Usuário deve pode apagar notas

Eu como usuária quero apagar uma nota para não a ver novamente.

***

##### Critérios de aceitação

O que deve acontecer para satisfazer as necessidades do usuário?

* Anotar um título em minha nota
* Adicionar o conteúdo da nota.
* Ver todas as minhas notas.
* Modificar as notas e ver a última modificação feita.
* Eliminar notas.
* Funciona bem em um _Tablet_

##### Definição de pronto

* Você deve ter recebido _code review_ de pelo menos uma parceira.
* Fez _testes_ unitários e, além disso, testou seu produto manualmente.
* Você fez _testes_ de usabilidade e incorporou o _feedback_ do usuário.
* Você deu deploy de seu aplicativo e marcou sua versão (tag git).

## 6. Considerações técnicas

O projeto deve conter os seguintes arquivos base de configuração,
ainda que não serão os únicos arquivos que terão que criar.

* `README.md` é onde se encontra a descrição do projeto e os elementos
  relevantes de seu projeto.
* `.editorconfig` com a configuração para o editor de texto. 
* `.gitignore` para ignorar o `node_modules` e outras pastas que não devem
  ser incluídas no controle de versão (`git`).
* `.eslintrc` este arquivo contém regras para formatar o 
código (configuração para o linter).
Além de ser uma boa prática ter configurado um linter.

Este projeto será uma Web App con **um
framework de JavaScript** (`React`) e **Firebase** para armazenar suas notas.

## 7. Hacker Edition

As seções chamadas _Hacker Edition_ são **opcionais**. Se você **terminou** tudo
e ainda sobrou tempo, faça essa parte. Assim você poderá aprofundar e exercitar
mais sobre os objetivos de aprendizagem do projeto.

* Se a usuária começa a escrever uma nota e por alguma razão a aba do
  navegador se fecha, a nota deve mostrar como
  estava, quando abrir novamente
* Subir imagens.
* Ver o número de vezes que a nota foi editada.
* Consumir API/s (Google Maps, Spotify, Pinterest, etc.)
* Progressive Web App (PWA).
* Criar categorias e classificar por tipo de nota.
* Guardar a color da nota.
* Criar uma nota publica.

## 8. Guias, dicas e leituras complementares

### Frameworks / bibliotecas

* [React](https://reactjs.org/)
* [React beta - versão em construção usando Hooks ](https://beta.reactjs.org/)
* [Create React App](https://create-react-app.dev/docs/getting-started)
* [Configuração inicial (vídeo)](https://youtu.be/38iZjr-jH5E)

### Ferramentas

* [npm-scripts](https://docs.npmjs.com/misc/scripts)
* [Babel](https://babeljs.io/)
* [webpack](https://webpack.js.org/)

### Rotas

* [React Router](https://reactrouter.com/web/guides/quick-start)

### PWA

* [Seu primeiro Progressive Web App - Google developers](https://developers.google.com/web/fundamentals/codelabs/your-first-pwapp/?hl=es)
* [Progressive Web Apps - codigofacilito.com](https://codigofacilito.com/articulos/progressive-apps)
* [Usando Service Workers - MDN](https://developer.mozilla.org/pt-BR/docs/Web/API/Service_Worker_API/Using_Service_Workers)
* [offlinefirst.org](http://offlinefirst.org/)
* [Como habilitar dados sem conexão - Firebase Docs](https://firebase.google.com/docs/firestore/manage-data/enable-offline)

### Deploy

* Veja a documentação [de deploy do Create React App](https://create-react-app.dev/docs/deployment).
Você pode utilizar qualquer um dos serviços listados na documentação,
sendo recomendado o Firebase, Vercel, Netlify, Github Pages ou Heroku.