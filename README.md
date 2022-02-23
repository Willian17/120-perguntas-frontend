
# 120-perguntas-frontend

  <br/><br/>

⬛ Níveis Junior, Pleno, Senior e Especialista

⬛ por Ruben Paschoarelli

⬛ Respondido por Willian

  <br/><br/>

`
Essas Perguntas/Respostas tem o intuito de ser uma base para entrevistas e candidatos se nivelarem, em entrevistas de emprego. Não são necessariamente o fator decisivo da senioridade de cada candidato, outros fatores como experiência em projetos, em liderança, documentação, saber caso de uso de tecnologia e conceitos, as vezes pode contar muito mais do que saber decor respostas para perguntas.
`

  <br/><br/>

### Outros Repositórios (em inglês)

[FrontEnd Developer Interview Questions](https://github.com/h5bp/Front-end-Developer-Interview-Questions)<br/>
[Vue.js Interview Questions](https://github.com/sudheerj/vuejs-interview-questions#what-is-vuejs)


## Junior

  

1.`O que é SQL injection?`<br/>
R: SQL Injection é uma vulnerabilidade de segurança, que consisten no invasor injetar ou manipular consultas SQL ao banco de dados relacional. Podendo causar consequências irreversíveis, com acesso dados sigilosos do sistema.

2.`O que é escopo em JavaScript?`<br/>
R: Escopo em Javascript é a acessibilidade de variaveis, objetos e funções em detereminada parte do código.

3.`Explique o CSS “box model” e os componentes de layout que o compõem.`<br/>
R: Em uma página Web, cada elemento é representado como um <string>box</strong> retangular. Determinar o tamanho, propriedades - como cor, fundo, estilo das bordas - e a posição desses boxes é o objetivo do mecanismo de renderização. Cada box possui 4 edges: margin, border, padding e content.

4.`Como JavaScript e jQuery são diferentes?`<br/>
R: Javascript é uma linguagem de programação, jQuery é uma biblioteca do Javascript focada na manipulação de elementos do DOM.

5.`O que é é um Callback Hell?`<br/>
R: Callback Hell é quando se tem várias callbacks dentro de outras callbacks, é um grande problema causado pela codificação com retornos aninhados complexos. Desta forma, a estrutura do código parece uma pirâmide, dificultando a leitura e manutenção. <br/>
```
getData(function(x){
    getMoreData(x, function(y){
        getMoreData(y, function(z){ 
            ...
        });
    });
});
```

6.`O que é Cross-Site Scripting (XSS)?`<br/>
R: É um ataque de injeção de client-side script (código malicioso) que se aproveita de brechas em aplicações web para se apropriar de dados no navegador.

7.`O que é Flux?`<br/>
R: É uma arquitetura de fluxo de dados usada pelo Facebook em conjunto com o framework React que propõe construir aplicações web no client-side que trabalha de forma reativa. Basicamente uma forma de fluxo unidirecional de dados entre eventos e ouvintes. Dividio em 4 partes: Views, Actions, Dispatcher e Stores
<ul>
  <li> <strong>Views</strong>: A interface do usuário, renderiza e cuida das interações com o usuário, de onde partirá os callbacks para criar as actions </li>
  <li> <strong>Actions</strong>: Eventos que passam dados para o dispatcher </li>
  <li> <strong>Dispatcher</strong>: Recebe os dados e envia para todos os stores registrado para ouvir aquela action </li>
  <li> <strong>Stores</strong>: Recebe as actions contendo os dados e emite eventos, eventos estes que irão atualizar os dados dos states, fazendo com que as views sejam renderizadas novamente </li>
</ul>

![image](https://user-images.githubusercontent.com/53010824/153788324-a2ccd688-1552-4bf1-a829-50efb8dc6dbf.png)


8.`O que é Sass?`<br/>
R: É uma linguagem de extensão do CSS, a sua ideia é adicionar recursos especiais como variáveis, mixins, funções, nested selectors. Tem o objetivo tornar o desenvolvimento mais simples e eficiente.

9.`O que é encapsulamento?`<br/>
R: Na programação orientada a objetos, o encapsulamento se refere à restrição do acesso direto aos atributos de um objeto.
```
  private String nome; 
  
  public String GetNome(){
    return nome;
  }
  public void SetNome(String nome){
    this.nome = nome;
  }
```

10.`Qual o ponto de se usar Redux?`<br/>
R: Com o redux é criado um state global, e todos os componentes tem acesso a esse state, isso elimina a necessidade de passar continuamente o state de um componente para outro.

11.`Explique a diferença de null e undefined em JavaScript`<br/> 
R: Null é um valor primitivo que representa a ausência intencional de um valor, ja o undefined é um valor primitivo utilizado quando não se teve valor atribuído previamente.

12.`Liste as vantagens da arquitetura de microsserviços`<br/> 
<ul>
  <li>Facilidade e rapidez na atualização e implantação dos serviços</li>
  <li>Aumentar a flexibilidade da infraestrutura</li>
  <li>Escalabilidade</li>
  <li>Estandardização de serviços</li>
  <li>Redução de dívida técnica</li>
  <li>Desenvolvimento de práticas de DevOps e de colaboração do time</li>
</ul>

13.`Quais são as vantagens do NoSQL sobre o RDBMS tradicional?`<br/>
<ul>
  <li>Escalabilidade</li>
  <li>Grande volume de Dados</li>
  <li>Flexibilidade no formato de dados</li>
  <li>Menor custo</li>
</ul>

14.`O que é programação reativa?`<br/>
R: É um paradigma de programação declarativo preocupado com os fluxos de dados e a propagação de mudança como o framework React.

15.`O que são os reducers no Redux?`<br/>
R: É encarregado de lidar com todas as ações e especificam como o estado da aplicação irá mudar de acordo com o action enviado para o store.

16.`Qual o papel do HTML na indexação de páginas por buscadores?`<br/>
R: Na indexação, se busca as páginas para o índice do motor de busca, motando o Pagerank, um ranking baseado numa fórmula desenvolvida pelo Google que considera também uma série de informações sobre o website para classificá-lo com uma pontuação de 0 a 10. O papel do HTML é muito influente nesse caso, quando mais semântico e bem escrito, melhor é o Pagerank, como os títulos das páginas, meta tags, heading tags, atributo alt em imagens e etc.

17.`Cite 3 conceitos da Programação Orientada a Objetos aplicada ao JavaScript`<br/> 
R: Classe, herança e encapsulamento.

18.`Quais os beneficios do TypeScript?`<br/>
R: Adiciona tipagem estática a linguagem JavaScript, possibilita que a IDE incremente o IntelliSense, Utilizar funcionalidades do Javascript que ainda não estão disponíveis de forma nativa, transpilar o código para que o mesmo seja lido por todas as versões do browsers.

19.`O que é uma interface no TypeScript?`<br/>
R: Uma interface é um conjunto de métodos e propriedades que descrevem o objeto, porém não incializa nem os implementa. Uma classe ou estrutura irá utilizar essa interface, sendo obrigada a implementar todos os seus membros.

20.`Qual o significado de Mock?`<br/>
R: São objetos que simulam o comportamento de objetos reais de forma controlada, são normalmentre criados para testar o comportamento de outros objetos reais.

21.`O que é o esquema do GraphQL?`<br/>
R: É composto por tipos de objetos que definem os objeto que podem ser solicitados e quais campos eles terão. Conforme a consulta são recebidas, o GraphQL as valida de acordo com o esquema. Em seguida executa as consultas validadas.

22.`O que é o Virtual DOM? Qual sua vantagem?`<br/>
R: Virtual DOM (VDOM) é uma representação do DOM mantida em memória. Assim quando precisamos fazer uma alteração, ela é feita no Virtual DOM, que é bem mais simples mais rápido que o DOM. Com isso ele analisa todos os lugares que serão afetados e sincroniza com o DOM em um processo chamado Reconciliação.

23.`O que é e como usar a convenção Block Element Modifier (BEM)?`<br/>
R: É um padrão do CSS para dar nomes a classes no css, para ter melhor relação entre HTML e o CSS. Onde 2 uderlines (__) são os elementos do bloco, será uma parte, complemento da estrutura do bloco, e 2 traços (--) são os modificadores do bloco, os estados que os bloco ou elemento poderão ter.

```
<ul class="list">
  <li class="list__item">
    <h2 class="list__item__title list__item--active">My publication</h2>
  </li>
</ul>
```



24.`JavaScript: Explique como você pode usar funções JavaScript, como forEach, Map, Filter e Reduce.`
R: forEach serve para percorrer um array, o Map para transformar/alterar items do array e no final retorna um novo array, O Filter filtra os elementos de acordo com a condição e retorna um array filtrado, o Reduce reduz de um array para um único elemento.


25.`React: O que é e como você pode aproveitar as vantagens do PureComponent?`<br/>
R: O PureComponent faz uma comparação superficial na mudança de estado, ao comparar valores escalares, ele compara seus valores, mas ao comparar objetos compara apenas a referência, isso ajuda a melhorar o desempenho da aplicação. Estado/adereços deve ser um objeto imutável, não devem ter uma hierarquia e deve ligar o forceUpdate quando os dados forem alterados.

26.`O que é serverless computing?`<br/>
R: Uma evolução do cloud computing, é um modelo de execução de computação em nuvem no qual o provedor de nivem aloca recursos da máquina sob demanda. O Serverless elimina uma camada operacional de servidores que estão sempre ligados e aloca recursos deles na nuvem.

27.`Quais são os tipos primitivos do JavaScript?`<br/>
R: String, Number, Boolean, Null, undefined, Symbol (ECMA 6)

28.`Qual a diferença entre inline and inline-block?`<br/>
R: O Inline ocuparão somente o espaço necessário para sua exibição, não será possível adicionar padding, margin, nem alterar o height e width, já o inline-block aceitam que seja definido os respectivos atributos css.

29.`Qual a diferença entre elementos posicionados como relative, fixed, absolute e static?`<br/>
R: 
<ul>
  <li><strong>Position Fixed:</strong> Irá fixar a posição do elemento na coordenada que você definir, independente se a página for rolada continuara sendo exibida.</li>
  <li><strong>Position Relative:</strong> Posiciona o elemento em relação a si mesmo</li>
  <li><strong>Position Absolute:</strong> Posiciona o elemento a partir dos elementos pai</li>
  <li><strong>Position Static:</strong> Valor padrão para os elementos, significa que vai seguir o fluxo da página normalmente</li>
</ul>



30.`Você pode explicar a diferença entre codificar um site para ser responsivo e usar uma estratégia mobile-first?`<br/><br/> 
R: Um site responsivo é que se adpta a qualquer dispositivo que o site for aberto, no modelo mobile-first é implementar pensando primeiramente na versão mobile.
  

## Pleno


1`.Mencione qual é a diferença entre PUT e POST?`<br/>
R: PUR/POST é um método Http. POST usado para adicionar informações, o PUT para alterar.

2.`O que são atributos defer e assync em uma tag <script>?`<br/>
R: Defer assim como occore com o async, com o defer o download do script é feito de forma assíncrona, mas sua execução ocorre apenas quando todo o processo de renderização estiver concluído.

3.``O que significa SOLID?  Quais são seus princípios?``<br/>
R: SOLID São princípios e boas práticas de programação que melhore o design de software e arquitetura, seus princípios são:
<ol>
  <li><strong>S</strong>ingle Responsiblity: Uma classe deve ter um, e somente um, motivo para mudar.</li>
  <li><strong>O</strong>pen-Closed: Objetos ou entidades devem estar abertos para extensão, mas fechados para modificação</li>
  <li><strong>L</strong>iskov Substitution: Uma classe derivada deve ser substituível por sua classe base</li>
  <li><strong>I</strong>nterface Segregation: Uma classe não deve ser forçada a implementar interfaces e métodos que não irão utilizar</li>
  <li><strong>D</strong>ependency Inversion: Dependa de abstrações e não de implementações</li>
</ol>

4.`O que é coerção em JavaScript?`<br/>
R: É um processo de conversão de um valor de um tipo, para outro (como a conversão de string para number). Qualquer tipo , seja primitivo ou um objeto, é um sujeito válido para coerção de tipo.

5.`SASS: O que é um Mixin e como usá-lo?` <br/>
R: Além de poder adicionar argumentos, um mixin pode fazer um bloco inteiro de estilos, conhecidos como bloco de contéudo, permitem definir estilos que podem ser reutilizados em toda folha de estilo, sem a necessidade de recorrer a classes não semânticas.
```
@mixin cabecalho($side-padding) {
  width: 100%;
  padding-left: $side-padding;
  padding-right: $side-padding;
  margin-bottom: 2em;
  @content;
}

header {
  @include cabecalho(1em) {
    background-color: blue;
  }
}
```

6.`Cite alguns sistemas de grid CSS`<br/>
R: grid-template-columns, grid-template-rows, grid-template-areas, grid-template, grid-auto-columns, grid-auto-columns.

7.`Quando devo usar as Arrow functions no ES6?`<br/>
R: Para funções que não sejam métodos, Em funções mais curtas, e quando não precisar usar o contexto(this, arguments, super, new.target).

8.`Quando devemos usar generators no ES6?`<br/>
R: Quando queremos uma função que pode ser executada, pausada e continuada em diferentes estágios da sua execução. Criar de maneira mais fácil iteradores e controlar o código assíncrono.

9.`Cite algumas características de sistemas reativos`<br/>
R: Flexíveis, desaclopados e escaláveis.

10.`Descreva a diferença entre a programação reativa e a programação imperativa`<br/>
R: Programação reativa reage a eventos disparados por interações do usuário ou situações comuns. Já a programação imperativa é mais autoritária, diz como e o quê exatamente um programa ou rotina deve realizar.

11.`Qual é a diferença entre Promises e Observables?`<br/>
R: Promisse processa um único evento quando uma operação assíncrona é concluída ou falha, já o Observable permite passar 0 ou mais eventos onde o callback é chamada a cada evento.

12.`Como acessar a store redux fora de um componente react?`<br/>
R: Exportar o store, e importar no client com store.getState().

13.`Quais são as desvantagens do Redux em relação ao Flux?`<br/>
R: Flux é independente em relação a mutação de dados, já o Redux, não é projetado para mutações. Flux permite fazer verificações por tipo estático, enquanto o Redux ainda não possui esse suporte.

14.`Qual a maneira correta de acessar a Redux store?`<br/>
R: Criar um provider envolvendo o component global, use o connect dentro do component global, e acesse a partir do this.props de cada component.
```
export default connect(mapStateToProps)(App);
```

15.`O que é "git cherry-pick"?`<br/>
R: O git cherry-pick é um podereso comando que permite que commits de Git arbitrários sejam coletados como referência e anexados ao HEAD de trabalho atual. Por exemplo, digamos que o commit seja feito sem querer na branch errada, é possível alterar para a branch correta e fazer cherry-pick do commit para onde devia pertencer.

16.`O que é um WebWorker?`<br/>
R: São mecanismos que permitem que uma operação de um dado script seja executado em uma thread diferente da thread principal da aplicação web. Permitindo que cálculos laboriosos sejam processados sem que ocorra bloqueio da thread principal.

17.`O que é o DOM?`<br/>
R: Document Object Model é utilizado pelo navegador web para representar uma página web.

18.`Qual a diferença de localStorage e sessionStorage?`<br/>
R: localStorage os dados não expiram, já os dados do sessionStorage tem seus dados limpos ao expirar a sessão da página.

19.`Como evitar callback hells?`<br/>
R: É separar em funções isoladas, guardar em uma variavel e usar como callback.

20.`O que é Injeção de Dependencia?`<br/>
R: É um padrão de projeto usado para evitar o alto nível de aclopamento. Módulos de alto nível não devem depender de módulos de baixo nível. Ambos devem depender de abstrações.

21.`O que é a keyword "new" em JavaScript?`<br/>
R: Permite que crie uma instância de um objeto.

22.`Explique o conceito de Server Side Rendering. Cite algum framework com esse proposito`<br/>
R: SSR é deixar de renderizar no client-side para ser rendereizado como estático do lado do servidor. Usado pelo framework NextJS.

23.`O que são Estrutura de dados e porque elas são importantes?`<br/>
R: É a organização de dados para atender aos diferentes requisitos de processamento. Existem as Listas, Árvores, grafos e Tabelas Hash.

24.`O que é renderização progressiva?`<br/>
R: Melhora o desempenho da página buscando e renderizando os componentes de maneira paralela e priorizada.

25.`Para que servem os data-attributes?`<br/>
R: Permite armazenar informações extras em elementos HTML padrões e semânticos, sem a necessidade de hacks como classList, atributos fora do padrão, propriedades extras no DOM ou método depreciado setUserData.

26.`Explique a diferença entre funções sincronas e assíncronas.`<br/>
R: Síncrona refere-se ao contato imediato entre o emissor e o receptor, a comunicação assíncrona é atemporal. Ou seja, o emissor envia a mensagem mas não necessariamente o receptor irá recebê-la imediatamente.

27.`Qual a diferença entre os métodos setTimeout e setInterval?`<br/>
R: setTimeout executa um bloco de código uma vez depois de um determinado tempo, já o setInterval executa o bloco repetidamente com um intervalo fixo entre cada chamada.

28.`O que é um construtor?`<br/>
R: É chamado assim que uma nova instância de objeto for criada.

29.`Qual a função dos prototypes no JavaScript?`<br/>
R: É um objeto implícito que está disponível para todas as funções construtoras do javascript, é um atributo da função Object, de onde as funções herdam.

30.`O que são High Order Functions`<br/>
R: São funções que recebem uma ou mais funções como argumento, e depois executar essa função passada ou até retorná-la para ser executada posteriomente, mais conhechido também como funções de callback, como o map(), filter(), reducer().

<br/> 



## Senior
1.`O que é  "closure" no javascript? Cite um exemplo?`<br/>

2.`Imperativo vs Funcional vs Programação Reativa.Explique`<br/>

3.`Você pode explicar o que “git reset” faz ?`<br/>

4.`Qual a diferença de Interface e Type no TypeScript?`<br/>

5.`O que é teste de unidade, teste de integração e quais são as diferenças entre eles?`<br/>

6.`O que é uma arvore de busca binária?`<br/>

7.`O que é o Shadow DOM e qual seu uso?`<br/>

8.`Qual a diferença entre os métodos apply.call e bind?`<br/>

9.`O que descreve o algoritmo de Big O Notation?`<br/>

10.`O que é o conceito de Immutabilidade?`<br/>

11.`Quais são boas práticas de Clean Code?`<br/>

12.`O que é o "HEAD" no Git?`<br/>

13.`Quais são as diferenças entre continuous integration, continuous delivery e continuous deployment?`<br/>

14.`Explique um caso de uso do  Docker`<br/>

15.`O que é o React Hooks?`<br/>

16.`Como você abordaria a correção de problemas de estilo específicos do navegador?`<br/>

17.`Angular: O que são lifecycle hooks para componentes e diretivas?`<br/>

18.`Explique o conceito de Lazy Loading`<br/>

19.`Quando se usar uma classe abstrata?`<br/>

20.`Explique o conceito de encapsulamento de dados`<br/>

21.`React: O que são fragments?`<br/>

22.`Porque você criaria classes estáticas?`<br/>

23.`Explique o CORS e como isso pode afetar um website.`<br/>

24.`Cite algumas vulnerabilidades de REST APIS`<br/>

25.`O que é JWT? Como implementar? Quais são as alternativas?`<br/>

26.`O que é Styled Components? Cite Alternativas`<br/>

27.`Dê exemplos de bibliotecas CSS in JS e suas vantagens e desvantagens`<br/>

28.`Dê exemplos de Convenções de código de JavaScript`  <br/>

29.`Quais as vantagens e desvantagens de programação funcional vs orientada a objetos?`<br/>

30.`O que é o  two-way data binding e o one-way data flow, e qual sua diferença?` <br/>   <br/> 


## Expert

1.`Cite algumas práticas recomendadas para um melhor design de API RESTful`<br/> 

2.`Programação Reativa: Explique Message-Driven vs Event-Driven`<br/> 

3.`Qual o modelo mental do redux-saga?`<br/> 

4.`Quando se usa "git rebase" ao invés de  "git merge"?`<br/> 

5.`O que são webcomponents?`<br/> 

6.`O que é ARIA?`<br/> 

7.`O que é um Hash Table?`<br/> 

8.`O que é o WebAssembly?`<br/> 

9.`Angular: compliação Just-in-Time (JiT) vs Ahead-of-Time (AoT).Explique a diferença.`<br/> 

10.`Qual a vantagem do incremental DOM  sobre o virtual DOM?`<br/> 

11.`OOP: Qual a diferença entre um mixin e uma herança?`<br/> 

12.`Como estilizar um elemento que está após o elemento selecionado?`<br/> 

13.`Explique como  'this' funciona no JavaScript`<br/> 

14.`Cite outros frameworks que fazem o mesmo que o React,Angular e Vue`<br/> 

15.`Qual dos dois é mais seguro, JWT ou OAuth2?`  <br/> 

16.`Como o  V8 compila o código JavaScript?`<br/> 

17.`O que é WCAG? Quais as diferenças de compliance A, AA, and AAA?`<br/> 

18.`O que é CSS BEM? Cite outros exemplos de Arquitetura CSS`<br/> 

19.`Quais os prós e contras de arquiteturas monolíticas vs microserviços?`<br/> 

20.`Qual o problema com o nesting do Sass? De algum exemplo.`<br/> 

21.`Fale as principais diferenças entre UX e UI Design`<br/> 

22.`O que é caching?`<br/> 

23.`Qual é o proposito do metodo OPTIONS em webservices RESTful?`<br/> 

24.`Quais ferramentas você usaria para encontrar um bug de performance em seu código?`<br/> 

25.`Explique a diferença entre layout, painting and compositing.`<br/> 

26.`O que é domain pre-fetching e como ajuda com performance?`<br/> 

27.`O que é CDN e quais os benefícios de usar uma?`<br/> 

28.`JS: O que é Currying? Dê um exemplo de aplicação`<br/> 

29.`ES6: Async-Await x Yield/Next Generator, cite exemplos e diferenças`<br/> 

30.`JS: O que é o  "use strict";? Quais vantagens e desvantagens?` <br/> 
