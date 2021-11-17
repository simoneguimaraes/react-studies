# React
- [Conceitos Iniciais](#conceitos)
- [Instalação](#instalacao)
- [JSX](#jsx)
- [Contador](#contador)

Referências: 
- [MDN Mozilla](https://developer.mozilla.org/en-US/docs/Learn/Tools_and_testing/Client-side_JavaScript_frameworks/Introduction)
- [Geekhunter](https://blog.geekhunter.com.br/como-aprender-react/)
- [JSX in Depth](https://reactjs.org/docs/jsx-in-depth.html)

## <a name="conceitos"></a> Conceitos Iniciais
- React é uma bibloteca JavaScript usada para construir interfaces (UI).
#### Vantagens
- Ele faz a experiencia de criar interfaces ficar muito mais fácil para o desenvolvedor.
- Para os usuários a experiencia tambem fica melhor, pois fica mais facil pro usuario encontrar as informacoes e usar a aplicaçao.
#### Componentes
- Tudo que voce constroi no React será baseado em componentes. Aí voce vai juntar esses componentes e combina-los para construir a aplicacao
- Fica mais fácil e rápido para desenvolver a aplicação, porque se voce quiser mudar a cor do botão na pagina de envio de produto, por exemplo, voce pode fazer isso facilmente mudando essa informacao no componente, que vai se refletir no restante da aplicacao.
#### Renderização
- No React, voce pode renderizar apenas parte da aplicacao. 

## <a name="instalacao"></a> Instalação
#### Node, VS Code, React Dev Tools
- Para checar que instalou o Node (node -v)
- Para criar o Create React App (npx create-react-app .)
- npm install
- npm start
- npm test (test runner)
- npm run build (para o deploy)

#### Pastas do VS Code
- Node_modules: library files
- Public: index_html, favicon, manifest
- Src (all the Application code)
  - CSS, JS files, test files, logos, images
  - Index.js (hooks the HTML file to JS)
  - ServiceWorker: offline node
- .gitignore (tells git what it needs to ignore, ex: node modules to the github repository)
- Package-lock.json: tells the version of every file in node modules, automatically generated
- Package.json: details of different applications and dependencies
- README.md: information on how to run our application

#### Deletar o que voce nao precisa
- Public: mudar o title (index.html) e remover --> favicon, index.html (favicon, theme-color, manifest-json, comments), manifest.json
- Src: index.js (index.css, serviceWorker, comments and serviceWorker), index.css, serviceWorker, App.js(index.css, serviceWorker, e tudo dentro do return - return null), app.css, app.test.js, logo

## <a name="jsx"></a>JSX
- Sintaxe que nos permite escrever HTML no Javascript
- Como o retorno possibilita ser de vários elementos, usamos o parenteses ()
```
function App() {
   return(
      <h1>Hello World</h1>
   )
}
```
Se fosse no DOM, precisaríamos escrever:
```
const title = document.createElement('h1')
title.innerText = 'Hello World'

```
O retorno precisa ser de uma única coisa. Entao voce pode envolver todos os elementos em uma 'div':
```
function App() {
   return(
      <div>
        <h1>Hello World</h1>
        <h3>Welcome to my page<h3>
      </div>
   )
}
```
Ou usar os fragments (<> </> brackets vazios)
```
function App() {
   return(
      <>
        <h1>Hello World</h1>
        <h3>Welcome to my page<h3>
      </>
   )
}
```
## <a name="contador"></a>Contador
```
function App() {
   return(
      <>
        <button>-</button>
        <span>0</span>
        <button>+</button>
      </>
   )
}
```
Class Component

















