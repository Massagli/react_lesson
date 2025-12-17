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


<ul>
    <li>Para instalar o React vamos utilizar uma ferramente chamada <b>Create React App</b>, usando o seguinte comando:</li>
    <ul><li>npm install -g create-react-app </li></ul>

</ul>
<ul>Recebemos todos os arquivos da biblioteca e <b>temos que executá-la</b>;</ul>
<ul>Para utilizar precisamos do <b>Node e npm</b>;</ul>
<ul>Esta ferramente também otimiza o app gerado para <b>produção</b>;</ul>

Sempre que fomos rodar algum comando, precisamos usar o npm ou npx que é o comando e execução.

<!-- -- -->

<h1>Criando o projeto</h1>
Para criar o projeto, no terminal do VSCODE precisamos colocar o seguinte comando "create-react-app [nome do projeto]";
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


<!-- -- -->


<h1>Props</h1>
<ul>As <b>props</b> são valores passados para componentes;</ul>
<ul>Podemos deixá-los <b>dinâmicos</b>;</ul>
<ul>Ou seja, <b>mudando a execução</b> por causa do valor da prop;</ul>
<ul>O valor é <b>passado como um atributo</b> na chamda do componente;</ul>
<ul>E precisa ser <b>resgatado dentro de uma propriedade/argumento</b> chamada props na função de definição do componente;</ul>
<ul>As props são somente de leitura.</ul>

<p>Em resumo, as props são argumentos dos componentes, onde podemos passar variáveis para deixá-lo dinâmico.</p>

<h3>Como criar uma prop</h3>
<p>Para criar uma prop basta escrever "props" passando como argumento no componente </p>

Exemplo: 

function SayMyName(props){  

    return(
        <div>
            <p>Fala aí {props.nome}, suave?</p>
        </div>
    )
}

<p>O ".nome" é como se fosse uma variável do um objeto</p>

<h3>Structure</h3>
<p>Há uma maneira mais inteligente para passar os argumento ao invés de usar a palavra "props". Podemos simplesmente passar os argumentos que vamos usar</p>

Exemplo: 

function SayMyName({nome}){  

    return(
        <div>
            <p>Fala aí {nome}, suave?</p>
        </div>
    )
}

<h1>Adicionando CSS</h1>
<ul>O <b>CSS</b> pode ser <b>adicionado de forma global</b> na aplicação, por meio do arquivo index.css por exemplo;</ul>
<ul>Porém é possível <b>estilizar a nível de componentes</b>;</ul>
<ul>Utilizando o <b>CSS modules</b> para isso;</ul>
<ul>Basta criar um arquivo como <b>"Componente.module.css"</b>;</ul>
<ul>E chamar este CSS no componente.</ul>

<h3>Criando CSS</h3>
<p>Para fazer alterações globais no css, utilizamos o arquivo index.css</p>
<p>Para fazer alterações apenas em um módulo, precisamos criar um arquivos css chamado [nome_do_módulo].module.css dentro da pasta de componentes</p>

Exemplo:

Pessoa.js
Pessoa.module.css

<p>Para importar para os estilos precisamos usar o import, assim como usamos para importar componentes. (Exemplo: import styles from '')</p>
<p>Para receber o estilo, precisamos colocar o nome da classe. (Exemplo: div className={styles.estilo}>/div></p>

<!-- -- -->

<h1>Fragmentos</h1>

<ul>Os React Fragments permite a criação de um componente sem elemento pai;</ul>
<ul>O propósito é descomplicar os nós do DOM;</ul>
<ul>A sintaxe é <> e </>, não há um nome para a tag;</ul>
<ul>Criamos no próprio JSX;</ul>

<!-- -- -->

<h1>Avançando em props</h1>

<ul>Podemos definir tipos para as props, realizando uma espécie de validação;</ul>
<ul>Definimos em um objeto chamado propTypes no próprio componente;</ul>
<ul>E ainda há a possibilidade de definir um valor padrão;</ul>
<ul>Neste caso utilizamos o objeto defaultProps;</ul>

<!-- -- -->

<h1>Eventos</h1>

<ul>Os eventos de react são os mesmo eventos do DOM;</ul>
<ul>Ou seja, temos eventos para responder a um click;</ul>
<ul>O evento é atrelado a uma tag que irá executá-lo;</ul>
<ul>Geralmente um método é atribuído ao evento;</ul>
<ul>Este método deve ser criado no componente.</ul>

<!-- -- -->

<h1>useState</h1>

<ul>O useState é um hook do React;</ul>
<ul>Com ele conseguimos manusear o estado de um componente de forma simples;</ul>
<ul>Este hook funciona muito bem com eventos;</ul>
<ul>Podemos atrelar um evento a mudança de state;</ul>

