# react_lesson

<h1>O que é REACT</h1>

- Uma <b>biblioteca JS</b> para criação de interface
- Utilizado para contruir <b>SPAs</b> (single Page Application);
- Baseado em <b>componentes</b>;
- Utiliza o <b>JSX</b> para renderizar HTML;
- E aplica o <b>Virtual DOM</b> para realizar as alterações de DOM;
- Podemos <b>adicionar a um projeto</b> ou criar um projeto com ele.

<!-- -- -->

<h1>Como instalar o React?</h1>

<ul>Para instalar o React vamos utilizar uma ferramente chamada <b>Create React App</b>;</ul>
<ul>Recebemos todos os arquivos da biblioteca e <b>temos que executá-la</b>;</ul>
<ul>Para utilizar precisamos do <b>Node e npm</b>;</ul>
<ul>Esta ferramente também otimiza o app gerado para <b>produção</b>;</ul>
<ul>É possível iniciar a aplicação com <b>npm star</b>.</ul>

Sempre que fomos rodar algum comando, precisamos usar o npm ou npx que é o comando e execução.

<!-- -- -->

<h1>Criando o projeto</h1>
Para criar o projeto, no terminal do VSCODE precisamos colocar o seguinte comando "create_react_app [nome do projeto]";
Após isso precisamos entrar na pasta usando o comando "cd [nome do projeto]";
E iniciar o app usando o comando "npm start".

Tudo que vamos modificar será feito no "app.js"

<!-- -- -->

<h1>Entendendo o JSX</h1>

<ul> O <b>JSX</b> é como um HTML, porém dentro do código JavaScript</ul>
<ul> É a principal maneira de escrever HTML com React;</ul>
<ul> Podemos <b>interpolar variáveis</b>, inserindo ela entre {};</ul>
<ul> É possível também <b>executar funções</b> em JSX;</ul>
<ul> Inserir <b>valores em atributos de tags</b> também é valido em JSX;</ul>

<p>Em resumo, usamos o JSX apenas para conseguir manipular o HTML nas funções do React.</p>

<!-- -- -->

<h1>Componentes</h1>

<ul>Permite <b>dividir a aplicação</b> em partes;</ul>
<ul>Os componentes <b>renderizam JSX</b>, assim como App.js (que é um componente);</ul>
<ul>Precisamos <b>criar um arquivo</b> de componente;</ul>
<ul>E <b>importá-lo</b> onde precisamos utilizar;</ul>
<ul>Normalmente ficam em uma pasta chamada <b>components</b>;</ul>

<p>No geral, os componentes são frações do código que carregam estilos diferentes. Podemos relacionar com classes, onde cada classe possui uma característica diferente</p>

<h3>Criando um componente</h3>

<li>Criar pasta "Components" dentro da pasta "src"</li>
<li>Criar um aquivo .js que será o componente</li>  
</br>
<p>Para o nome do componente, devemos seguir o padrão PascalCase (primeira letra de cada palavra em maiúsculas) tanto para o nome do componente quanto para o nome do arquivo, por exemplo, UserProfile.js para o componente UserProfile.</p>
<p>O nome da função deve ser o mesmo nome do arquivo.</p>
<p>No final do arquivo devemos colocar o <b>"export defacult [função]"</b></p>

<h3>Importando componentes</h3>

<p>Para importar os componentes, precisamos ir no arquivo principal e o usar o comando "Import" (import HelloWorld from './components/HelloWorld')</p>
<p>Para chamar ele no código, basta abrir uma tag do html normal, usando o nome que demos no import (< HelloWorld/>)</p>

