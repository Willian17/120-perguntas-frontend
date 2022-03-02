
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
R: É um paradigma de programação declarativo preocupado com os fluxos de dados e a propagação de mudança, reage a eventos disparados por interações do usuário ou situações comuns.

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
R: Uma closure trata-se uma função que tem acesso a variaveis de sua função parente
```
function start() {
    var message = "hello world";

    function display() {
        console.log(message);
    }

    display();
}
start() // hello world
```

2.`Imperativo vs Funcional vs Programação Reativa. Explique`<br/>
R: Imperativo descreve exatamente como um programa ou rontina deve funcionar, controlando totalmente o estado do programa, A funcional usa a composição de funções puras evitando o compartilhamento de estados, dados mutáveis e efeitos colaterais, Programação reativa reage a eventos disparado pelo usuário ou situações comums do programa.

3.`Você pode explicar o que “git reset” faz ?`<br/>
R: Desfazer alterações locais no estado de um repositório git, gerenciando o estado interno do git como a árvore de commits(HEAD), o índice de staging e o diretório de trabalho.

4.`Qual a diferença de Interface e Type no TypeScript?`<br/>
R: Usar type é como se criasse um apelido para tipos primitivos. Interface para descrever uma forma de dados.

5.`O que é teste de unidade, teste de integração e quais são as diferenças entre eles?`<br/>
R: Teste de unidade é quando os módulos são testados individualmente, no de integração os módulos são combinados e testado em grupo.

6.`O que é uma arvore de busca binária?`<br/>
R: Uma árvore de busca binária é uma estrutura de dados baseada em nós, onde todos os nós da subárvore esquerda possuem valor numérico inferior ao nó raiz, e todos os nós da subárvore direita possuem um valor superior ao nó raiz.

![image](https://user-images.githubusercontent.com/53010824/155825371-9fa09778-c0f8-4f03-a822-800e8a9d6393.png)


7.`O que é o Shadow DOM e qual seu uso?`<br/>
R: É a que consiste em um subconjunto de nós do DOM com escopo próprio, quer dizer que o HTML, CSS e JS serão isolados do resto dos nós irmãos.

8.`Qual a diferença entre os métodos apply, call e bind?`<br/>
R: São todas funcões que tem o objetivo de executar uma função passando por ela diferente contexto e argumentos
<ul>
  <li> call: contexto, param1, param2, param3 </li>
  <li> apply: contexto, [param1, param2, param3] </li>
  <li> bind: contexto, param1, param2, param3. Porém cria uma instância da função, retornando ela </li>
</ul>

```
const pessoa = {
    idade: 15,
    apresentar: function(nome) {
        console.log(`Olá, meu nome é ${nome} e tenho ${this.idade} anos.`)
    }
}

pessoa2 = {
    idade: 18
}

pessoa.apresentar('Willian') // Olá, meu nome é Willian e tenho 15 anos.
pessoa.apresentar.call(pessoa2, 'Willian Call') // Olá, meu nome é Willian Call e tenho 18 anos.
pessoa.apresentar.apply(pessoa2, ['Willian Apply']) // Olá, meu nome é Willian Apply e tenho 18 anos.
pessoa.apresentar.bind(pessoa2, 'Willian Bind')() // Olá, meu nome é Willian Bind e tenho 18 anos.
```

9.`O que descreve o algoritmo de Big O Notation?`<br/>
R: É usada para classificar algoritmos em relação as mudanças de desempenho quanto ao tamanho da entrada. É um método de descrever o comportamento de limites, matematicamente falando.

![image](https://user-images.githubusercontent.com/53010824/155853867-d748912a-fb9b-40c2-b024-80238ff46cd4.png)

10.`O que é o conceito de Imutabilidade?`<br/>
R: É algo que não pode ser alterado.

11.`Quais são boas práticas de Clean Code?`<br/>
<ol> 
  <li>Nomes são muito importantes: Variaveis, funções, parâmetro, classe bem descritivos</li>
  <li>Regra do escoteiro: Deixar o código mais limpo do que quando você encontrou</li>
  <li>Seja o verdadeiro autor do código: Funções simples, claras e pequenas</li>
  <li>DRY: Não repetir código</li>
  <li>Comente apenas o necessário</li>
  <li>Tratamento de erros: As coisas podem dar errado mas deve continar fazendo o que precisa.</li>
  <li>Teste limpos: Testes rápido, independente, repetido em diversos ambientes, testar todas as condições. </li>
</ol>

12.`O que é o "HEAD" no Git?`<br/>
R: Significa a "branch atual".

13.`Quais são as diferenças entre continuous integration, continuous delivery e continuous deployment?`<br/>
R: CI (Continuous integration) é uma abordagem para testar cada mudança de código automaticamente, enquanto CD(Continuos Delivery) é uma abordagem para obter mudanças de novos recursos, configurações e correções de bugs. E o Continuous deployment é uma abordagem para validar se estão corretas e estáveis para o ambiente de produção.

![image](https://user-images.githubusercontent.com/53010824/155854360-aec13b08-9006-41c8-8a8d-8867d8aa81e3.png)


14.`Explique um caso de uso do  Docker`<br/>
R: Uma vez que a aplicação seja transformada em uma imagem Docker, ela pode ser instanciada como container em qualquer ambiente que desejar. Isso significa que poderá utilizar sua aplicação no notebook do desenvolvedor da mesma forma que é executada no servidor de produção.

15.`O que é o React Hooks?`<br/>
R: Hooks são funcões que permitem ligar-se aos recursos do state e ciclo de vida do React a partir de componentes funcionais.

16.`Como você abordaria a correção de problemas de estilo específicos do navegador?`<br/>
R: Propriedades como -moz, -ms, -o, -webkit no css para colocar compatibilidade no navegador

17.`Angular: O que são lifecycle hooks para componentes e diretivas?`<br/>
R: Todo componente no angular tem um conjunto de eventos de ciclo de vida(lifecycle hooks) que ocorrem quando um componente é criado, renderizado, tem o valor de suas propriedades alterados ou é destruido. O Angular invoca uma séries de métodos(hooks) como o ngOnChanges, ngOnInit, ngDoCheck, ngAfterContentInit, ngAfterContentChecked,  ngAfterViewInit, ngAfterViewChecked, ngOnDestroy.

18.`Explique o conceito de Lazy Loading`<br/>
R: É uma técnica de otimização de desempenho de páginas que tem como objetivo fazer com que conteúdos mais pesados sejam carregados de forma assíncrona ou condicional.

19.`Quando se usar uma classe abstrata?`<br/>
R: Quando todas as classes de uma hierarquia podem ser instanciadas, Hierarquia não tão estreitamente relacionados e especificar um comportamento de algo e não o tipo deste.

20.`Explique o conceito de encapsulamento de dados`<br/>
R: Significa evitar que sofram acessos indevidos. Onde contém métodos para gerenciar esses dados.

21.`React: O que são fragments?`<br/>
R: Permite agrupar uma lista de filhos sem adicionar nós extras ao DOM.

22.`Porque você criaria classes estáticas?`<br/>
R: Usadas no caso de não houver comportamento ou dados na classe que depende da identidade do objeto, para manter métodos não associados com um objeto específico.

23.`Explique o CORS e como isso pode afetar um website.`<br/>
R: Significa Cross-origin Resource Sharing (ou Compartilhamento de Recursos de Origem Cruzada) é um mecanismo utilizado pelos navegadores para compartilhar recursos entre diferentes origens. O CORS é uma especificação do W3C e fez uso de headers HTTP para informar aos navegadores se determinado recurso pode ou não ser usado.

24.`Cite algumas vulnerabilidades de REST APIS`<br/>
R: Injeção de código, ataques de solicitação de replay, ataques de falsificação, autenticação de usuário quebrada.

25.`O que é JWT? Como implementar? Quais são as alternativas?`<br/>
R: JWT (JSON Web Tokens) é um método RTC 7519 padrão da indústria para realizar autenticação entre duas partes por meio de um token assinado que autentica uma requisição. Gerar um token assinado, e quando receber de volta no header da requisição verificar se o token é válido. As alternativas são: OAuth2, Fernet, Branca e PASETO.

![image](https://user-images.githubusercontent.com/53010824/155856558-fbb21a17-fb41-4431-886f-d6e4a3c6ab66.png)

26.`O que é Styled Components? Cite Alternativas`<br/>
R: É uma biblioteca que utliza o conceito de CSS-in-JS, ou seja, que nos permite escrever códigos CSS dentro do Javascript. As alternativas são: Linaria, Css Blocks, Stitches,  Styletron, Emotion, Fela, Goober.

27.`Dê exemplos de bibliotecas CSS in JS e suas vantagens e desvantagens`<br/>
R: 

<ul> 
  <li>Linaria: Estilo baseado em prop dinâmico, CSS SourceMap, Linting CSS, porém dificil de implementar e configurar o bundler.</li> 
  <li>Astroturf: Flexibilidade, Suporte de adereços porém Documentação deficiente, dificil implementação. </li>
</ul>


28.`Dê exemplos de Convenções de código de JavaScript`  <br/>
R: As Variáveis e funções devem ter o nome em camelCase, espaço em torno de operadores, sempre usar 4 espaços de recuo de bloco de código. 

29.`Quais as vantagens e desvantagens de programação funcional vs orientada a objetos?`<br/>
![image](https://user-images.githubusercontent.com/53010824/155866729-61aca6fc-06be-496b-83f5-5fb85657a42c.png) 

30.`O que é o  two-way data binding e o one-way data flow, e qual sua diferença?` <br/> 
R: Two-way data binding é bidirecional vincula os dois lados: o model e a view, significa que quando um muda, o outro também muda e obtém o mesmo valor. Já o one-way data flow é unidirecional, a view vai sempre obter o estado a partir do model, para atualizar a view deverá primeiro mudar o model e, em seguida redesenhar a view.

<br/> 


## Expert

1.`Cite algumas práticas recomendadas para um melhor design de API RESTful`<br/> 
<ol> 
  <li>Um Recurso deve ser um substantivo e não um verbo </li>
  <li> Documentar API </li>
  <li> Sempre utilize JSON  </li>
  <li> Padronizar a entrada de dados </li>
  <li> Usar HTTPS </li>
  <li> Utilizar Query Params em filtros</li>
  <li> Cache e Autenticação </li>
  <li> Use logs </li>
  <li> Tenha métricas da API </li>
  <li> Mensagens de erros descritivas </li>
 
</ol>

2.`Programação Reativa: Explique Message-Driven vs Event-Driven`<br/> 
R: No message-driven cada componente tem um endereço exclusivo para que outros componentes podem enviar. Cada um desses componentes ou destinatários, aguarda mensagens e reage a ele. Um Event é alguns dados emitido a partir de um componente para quem possa consumir. 

3.`Qual o modelo mental do redux-saga?`<br/> 
R: Uma saga é como uma thread separada da aplicação que é unicamente responsável por side effects. Redux saga é um redux middleware, que significa que essa thread possa ser estartada, pausada ou cancelada na aplicação principal.

4.`Quando se usa "git rebase" ao invés de  "git merge"?`<br/> 
R: Se preferir um histórico limpo, linear e sem commits de mesclagem desnecessários, pode usar git rebase em vez de git merge ao integrar alterações de outra ramificação.

5.`O que são webcomponents?`<br/> 
R: É uma suíte de diferentes tecnlogias que permite a criação de elementos customizados reutilizáveis e que podem ser utilizados em aplicações web.

6.`O que é ARIA?`<br/> 
R: O ARIA é um conjunto de atributos especiais de acessibilidade, que pode ser adicionado a qualquer linguagem de marcação, mas é especialmente adequado para HTML. O Atributo da função define qual é o modelo de objeto (tais como artigo, um alerta, ou algo que deslize). Há atributos adicionais ARIA que forncecem outras propriedades úteis, como o valor atual de uma barra de progresso.
```
<li tabindex="0" class="checkbox" role="checkbox" checked aria-checked="true">
  Receive promotional offers
</li>
```

7.`O que é um Hash Table?`<br/> 
R: É uma estrutura de dados especial, que associa chaves de pesquisa a valores. Seu objetivo é, a partir de uma chave simples, fazer uma busca rápida e obter o valor desejado.
![image](https://user-images.githubusercontent.com/53010824/155906684-278c0351-931d-4aa0-95b8-d57750b04643.png)


8.`O que é o WebAssembly?`<br/> 
R: WebAssembly é uma linguagem de baixo nível do tipo assembly com um formato binário compacto, que é executado com perfomance próxima a nativa, que disponibiliza linguagens com modelos de memória de baixo nível como C++ e Rust, com uma compilição-alvo, assim pode ser executado na web.

9.`Angular: compliação Just-in-Time (JiT) vs Ahead-of-Time (AoT).Explique a diferença.`<br/> 
R: No JIT, que era o padrão do angular até a versão 8, esta compilação é realizada no browser, em tempo de execução. Ou seja, quando o site é acessado, o Browser baixa os arquivos javascript ainda não compilados, baixa também o compilador do Angular, executa a compilação e, finalmente, mostra o resultado para o usuário.
Já no modo AOT, está compilação é feita durante o build, Ou seja o browser já obtem o JavaScript pré-compilado, sem a necessasidade de compilar o código ou mesmo baixar o compilador Angular.

10.`Qual a vantagem do incremental DOM  sobre o virtual DOM?`<br/> 
R: O DOM incremental traz uma solução para reduzir o consumo no DOM virtual usando DOM real para rastrear alterações. Essa abordagem reduziu drasticamente a sobrecarga de cálculo e melhorou o uso de memória dos aplicativos.

11.`OOP: Qual a diferença entre um mixin e uma herança?`<br/> 
R: A herança faz subtipo e sublasse, o mixins só faz apenas subclasse, portanto há uma inclusão e não uma herança.

12.`Como estilizar um elemento que está após o elemento selecionado?`<br/> 
R: Usando o seletor `+`
```
div + p
```

13.`Explique como  'this' funciona no JavaScript`<br/> 
R: O this faz refeência ao objeto que está chamando a função no momento. Em Javascript você pode usar this no contexto global e no contexto de função. Além disso, o comportamento do this muda entre o modo estrito e não estrito, no contexto global o this faz referência ao objeto global, que é window no navegador e global no Node.js, no modo estrito define o this como undefined.

14.`Cite outros frameworks que fazem o mesmo que o React,Angular e Vue`<br/> 
R: Petit DOM, Surplus, RE: DOM, Mithrill, Bobril, Marko, Nest, Svelte, Hapi.js, Koa e Ember.

15.`Qual dos dois é mais seguro, JWT ou OAuth2?`  <br/> 
R: São duas coisas diferentes, OAuth2 define um protocolo de autenticação, ou seja, especifica como os tokens são transferidos, Já o JWT define o formato de token.

16.`Como o  V8 compila o código JavaScript?`<br/> 
R: O motor V8 usa a compilação Just in Time (JIT), inicialmente usa um interpretador para interpretar o código. Em outras ocasiões, o motor V8 encontra padrões e os compila para melhorar o desempenho.

17.`O que é WCAG? Quais as diferenças de compliance A, AA, and AAA?`<br/> 
R: O critérios do WCAG visam tornar o conteúdo mais acessível a um público mais amplo de pessoas com deficiência.
<ul> 
  <li> Nível A: estão critério simples que representam apenas barreiras mais significativas de acessibilidade./li>
  <li> Nível AA: apresenta para a maior parte dos usuários garantindo acesso à grande maioria dos conteúdos./li>
  <li> Nível AAA: refinamento das anteriores sendo especificações mais detalhadas e que trazem de um nível mais sofisticado de acessibilidade/li>
</ul>

18.`O que é CSS BEM? Cite outros exemplos de Arquitetura CSS`<br/> 
R: É um padrão do CSS para dar nomes a classes no css, para ter melhor relação entre HTML e o CSS. É um acrônimo para Bloco, Elemento e Modificador, assim como existe o OOCSS (CSS orientado a objetos) e RSCSS (Sistema razoável para estrutura CSS).

19.`Quais os prós e contras de arquiteturas monolítica e microsserviços?`<br/> 
R: Monolítica é mais simples de desenvolver, testar e deploy para o servidor, além de ser simples de escalar. Porém é mais difícil a manutenção, fazer alterações, e mais chances de acontecer bugs. <br> Já os microsserviços é independentemente desenvolvido e escalável, pode ser reutulizado em múltiplas aplicações. Porém é mais complexo de se implementar,  e no gerenciamento da aplicação, será necessário ser padronizado para todo o projeto.

20.`Qual o problema com o nesting do Sass? De algum exemplo.`<br/> 
R: Geração de códigos inútil, aumentando o tamanho do arquivo final e principalmente a quebra de especificidade e a herança do código CSS.
```
  main {  
   .one {  
     .two {  
       a {
         color: red
       }  
     }
   }  
  }
```

21.`Fale as principais diferenças entre UX e UI Design`<br/> 
R: UI Design tem como foco principal foco a interface de um determinado aplicação, como o usuário interage. Já o UX Design cuida da experiência do usuário, o sentimento do usuário com a interação.

![image](https://user-images.githubusercontent.com/53010824/156059339-199fe580-af71-4174-947b-d8d23a0239ff.png)

22.`O que é caching?`<br/> 
R: É uma camada de armazenamento físico de dados de alta velocidade que guarda um subconjunto de dados, geralmente temporário, para que futuras solicitações sejam atendidas de modo mais rápido do que é possível fazer ao acessar o local de armazenamento principal de dados.

23.`Qual é o proposito do metodo OPTIONS em webservices RESTful?`<br/> 
R: É utilizado para que um cliente possa descobrir quais as opções de requisições permitidas para um determinado recurso em um servidor.
```
curl -X OPTIONS http://example.org -i
```

```
HTTP/1.1 200 OK
Allow: OPTIONS, GET, HEAD, POST
Cache-Control: max-age=604800
Date: Thu, 13 Oct 2016 11:45:00 GMT
Expires: Thu, 20 Oct 2016 11:45:00 GMT
Server: EOS (lax004/2813)
x-ec-custom-error: 1
Content-Length: 0
```

24.`Quais ferramentas você usaria para encontrar um bug de performance em seu código?`<br/> 
R: FindBugs, PMD, Kinsta APM, WebLOAD, Loadero, StormForge, Silk Performer, Gatling, Loadster, Locust.

25.`Explique a diferença entre layout, painting and compositing.`<br/> 
<ul>
   <li>Layout: A maneira como as partes de elementos são dispostas</li>
   <li>Paiting: É o processo de preenchimento de pixels, cores, imagens, bordas, sombras e etc, concluída em várias camadas.</li>
   <li>Compositing: Combina todas as camadas em uma camada em ordem correta e exibe na tela. </li>
</ul>

26.`O que é domain pre-fetching e como ajuda com performance?`<br/> 
R: É tentar resolver o DNS de quaisquer links existentes em uma página de forma antecipada, melhorando consideravelmente a perfomance.

27.`O que é CDN e quais os benefícios de usar uma?`<br/> 
R: CDN(Content Delivery Network) é uma rede de servidores que está distribuída em vários pontos do mundo, em diversos data centers localizados em pontos estratégicos, para armazenar conteúdos estáticos de sites, reduzindo a latência e agilizar a entrega destes dados ao usuário final.

28.`JS: O que é Currying? Dê um exemplo de aplicação`<br/> 
R: É o processo de transformar uma função que espera vários argumentos em uma função que espera um único argumento e retorna outra função curried.

```
function produto(a) {
    return function(b) {
        return a * b;
    };
}
console.log(produto(2)(8)); // 16
```

29.`ES6: Async-Await x Yield/Next Generator, cite exemplos e diferenças`<br/> 
```
async function testeAwait() {
    const users = await getUsersFromDatabase();
    return users + "Corretamente retornado";
}
```
Generators são funções pausadas que podem gerar valores sob demanda, sempre que o objeto iterador solicitar o próximo valor.
```
function* testeGenerator() {
    const users = yield getUsersFromDatabase();
    return users + "Corretamente retornado";
}

const iterator = testeGenerator();
const iteration = iterator.next();

iteration.value.then(result => {
    const nextIteration = iterator.next(result); // value: 'Test Users Corretamente retornado' done: true
})
```

30.`JS: O que é o  "use strict";? Quais vantagens e desvantagens?` <br/> 
R: É o modo estrito, que previne algumas ações de serem tomadas e envia mais exceções, é como se fosse uma versão mais segura e reduzida do JavaScript. Gera mais erros e desabilita alguns recursos em um esforço para tornar o código mais robusto, legível e preciso.
