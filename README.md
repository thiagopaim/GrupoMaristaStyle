# GrupoMaristaStyle
Este documento é um manual de boas práticas para front-end, usabilidade e acessibilidade. Tem o intuito de padronizar os códigos e as interfaces produzidas pelo Grupo Marista, levando em consideração cada projeto.

Os exemplos apresentados são fundamentados  e utilizados por grande empresas com grande relevância no mercado, como Github, Twitter, W3C e Tableless. Contudo, não são regras. É um arquivo aberto para qualquer tipo de colaboração relevante ao assunto.

#CSS

Espaçamentos
Nunca misture tabs e espaços na indentação. Escolha apenas um e utilize. De preferência utilize tabs;
Se optar por  espaços,  utilizer quatro;
Sempre adicione espaço após o : nas declarações de propriedade;
Sempre adicione espaço antes do colchete de abertura ( { ) nas declarações de propriedade;
Sempre colocar o colchete de fechamento ( } ) em uma linha separada;
Elimine os espaços vazios na quebra de linha;
Quando utilizar grupo de seletores, adicione um para cada linha. Exemplo 1;

Exemplo 1:
.classe1,
.classe2,
.classe3 {
    display: block;
}

Cores
Use preferencialmente cores hexadecimais #000, utilizar rgba(0, 0, 0, 0.5) apenas quando houver necessidade de transparência;
É recomendado o uso de apenas três dígitos para cores hexadecimais, quando for possível, como no exemplo acima.
Estrutura
Preferimos utilizar aspas duplas no código CSS;
Não utilizamos código em apenas uma linha, cada atributo deve ficar em uma linha;
Reutilize as classes sempre que possível.

Comentários
Para blocos de seção, utilize:
/* menu principal
---------------------------- */

Para subseção, utilize:
  /* busca ----------------- */

Não recomendamos utilizar comentários na mesma linha da propriedade:
p { color: #333 /* assim não é legal */ }
p { margin: 0; } /* assim não é legal */

Prefira comentários assim:
p {
    margin: 0;
    /* precisei comentar aqui para indicar algo */
    padding: 0;
    color: #fff;
}

Ordem das declarações
Se possível, utilize essa ordem hierárquica. Dentro da hierarquia, manter ordem alfabética dos atributos:
Posicionamento
Box model (width, height, padding e margin)
Tipografia
Visual

Sugestão
Leitura: http://sergiolopes.org/css-box-sizing-border-box/

#PUCPR Padrões CSS

Fontes

A velha e boa Arial funciona bem para sistemas. 

Podemos utilizar font-family: Helvetica, Arial, san-serif;

Tamanho
Texto Normal - VERIFICAR REM, EM OU PX
html: 100%;
font-size: 1.25rem;
line-height: 1.6;
Títulos
h1 - font-size: 2.44444rem;
h2 - font-size: 2.05556rem;
h3 - font-size: 1.5rem;

Sugestão
Acessibilidade: Verifique sempre o contraste entre texto e background. Ferramenta: http://webaim.org/resources/contrastchecker/

Cores Backgrounds e Links
Bordô PUCPR
Hexadecimal: #AA2439
RGB: 170, 36, 57

Caso o link esteja em um fundo mesma cor apresentada a cima, utilize branco;
Azul Grupo Marista
Hexadecimal: #005288
RGB: 0, 82, 136

Caso o link esteja em um fundo mesma cor apresentada a cima, utilize branco;

#Responsividade

Tempo é precioso, então para agilizar o processo em websites institucionais utilizamos o framework Foundation: http://foundation.zurb.com, incluindo as webfonts que ele utiliza.

A documentação completa pode ser encontrada em http://foundation.zurb.com/docs/index.html

#Grid

Small Screens
Medium Screens
Large Screens
XLarge Screens
XXLarge Screens

largura
< 640
> 641 e < 1024
> 1025 e < 1440
> 1441 e < 1920
> 1921

grid
12 colunas

Entre colunas
L: 15 - R: 15 - pixels

Media Queries
Small screens
max-width 640px, mobile-only styles

Medium screens
min-width 641px, medium screens
min-width 641px and max-width 1024px

Large screens
min-width 1025px, large screens
min-width 1025px and max-width 1440px

XLarge screens
min-width 1441px, xlarge screens
min-width 1441px and max-width 1920px

XXLarge screens
min-width 1921px, xxlarge screens

O elemento .row é pai das colunas, definindo um conjunto de grids;
O elemento .column define apenas uma coluna no elemento .row;
O elemento .columns define várias colunas dentro no elemento .row;
O elemento .row tem uma margin de 15 pixels negativos para perfeito alinhamento das colunas;
A classe .colapse remove o espaço entre colunas.

#Formulários
Utilizar label indicando os campos (inputs e textareas).
Para relacionar um label com um input utilize <label for=”iddoinput”>
Adicionar tabindex para ordenação dos campos.
Deixar claro quais os campos são obrigatórios.
Aplicar padding nos campos input (text) e textarea, caso o framework não aplique. 7 pixels
Indicar em qual campo o usuário está destacando a borda ou mudando de cor o backgroud dos campos, desde que não interfira no contraste entre texto e fundo.
A altura e largura dos campos deve ser feita no css, não no html.

#Botões
As cores dos botões devem seguir a cor padrão do sistema.
Utilizar ações que contemplem as três ações de links e botões default, hover e active, via CSS.

Classe button
Adicionar cursor: pointer;

Mensagens de Alerta
Dividimos em três categorias as mensagens de alerta:

Mensagem de Sucesso
padding: 12px;
color: #fff;
background: #43ac6a;
border: 1px solid #3a945b;

Mensagem de Cuidado
padding: 12px;
color: #fff;
background: #f08a24;
border: 1px solid #de770f;

Mensagem de Erro
padding: 12px;
color: #fff;
background: #f04124;
border: 1px solid #de2d0f;

#Usabilidade

Por que usabilidade é importante?
Se um site ou sistema for difícil de usar, o usuário sai.
Se a página principal não for clara o suficiente para mostrar o que o sistema ou empresa tem a oferecer e o que é possível fazer, o usuário sai.
Se o usuário se perder, ele sai.
Se demorar para carregar, ele definitivamente sai.

Vantagens para Empresa?
Menor custo de desenvolvimento
Menor custo de manutenção
Retenção de consumidores
Diminuição na taxa de abandono
Maior eficiência
Menor custo de treinamento
Menor número de chamadas no call-center

Metas da Usabilidade
Facilidade de Aprendizagem
O usuário consegue rapidamente explorar o sistema e realizar as tarefas
Efetividade
Aumento de produtividade em função da curva de aprendizado
Memorização
Os usuários memorizam suas tarefas sem sobrecarga de interação
Flexibilidade
O sistema e a interface devem ser flexíveis aos erros do do usuário
Eficiência
Menos trabalho, mais resultado.
Satisfação
Conforto, segurança e felicidade subjetiva.



Testes de Usabilidade
O teste de usabilidade é um processo no qual participantes representativos
avaliam o grau que um produto se encontra em relação a critérios específicos de
usabilidade.

O referido teste pode servir para diferentes propósitos que envolvem tipos de
tarefas, medidas de performance e disposição de escalas, entrevistas ou inspeções a
serem aplicadas, buscando encontrar problemas de usabilidade e fazer recomendações
no sentido de eliminar os problemas e melhorar a usabilidade do produto, ou com a
finalidade de se comparar dois ou mais produtos.

Com a realização de testes de usabilidade, pode-se registrar os melhores
resultados obtidos para futuras realizações levando à minimização do custo do serviço
de suporte aos usuários, crescimento de vendas e prever o lançamento de produtos com
menos problemas de usabilidade e mais competitivos.

Segundo [RUB 94], testes de usabilidade são mais eficientes quando
implementados como parte do processo de desenvolvimento de um produto. Portanto,
uma forma interessante de determinar os tipos de testes é através do ciclo de vida de
desenvolvimento de um produto. Desta forma, se alguma deficiência é perdida em um
teste, um outro ciclo de teste oferece a oportunidade para identificar esta deficiência.

Teste de Exploração
O teste de exploração é efetuado quando o produto ainda se encontra em um
estágio preliminar de definição e desenho. Neste estágio, o perfil do usuário e a análise
de tarefas provavelmente estarão definidos. A fase de especificação poderá estar
completa e a fase desenho estará apenas começando.

O objetivo do teste de exploração é avaliar a efetividade do desenho preliminar e
conhecer a concepção do usuário ou modelo mental do produto.

 O processo para este tipo de teste é bastante informal, interagindo o participante
e o avaliador. Uma representação do software pode ser realizada através de uma
simulação do protótipo representando o layout básico, organização, funções e macro
operações.

Teste de Avaliação
Provavelmente o mais comum, simples e direto dos testes, podendo ser
conduzido no início ou no meio do ciclo de desenvolvimento do produto, geralmente
depois que o desenho fundamental ou organização do produto foi estabelecido.
Seu propósito é expandir o que foi conseguido no teste de exploração avaliando
a usabilidade em um nível baixo de operações e aspectos do produto. Baseando-se no
modelo conceitual do produto, este teste busca examinar e avaliar como o conceito foi
implementado efetivamente, verificando como um usuário consegue desenvolver tarefas
reais, identificando deficiências específicas de usabilidade.

O usuário executa tarefas bastante simples caminhando entre as telas onde é
dada mais ênfase ao comportamento. Medidas quantitativas são coletadas.

Teste de Validação
Realizado mais tarde no ciclo de desenvolvimento, o teste de validação certifica
a usabilidade do produto bem próximo de sua liberação.

Seu objetivo é verificar como o produto se enquadra em relação a padrões de
usabilidade, padrões de performance e padrões históricos. Esses padrões são originados
dos objetivos de usabilidade definidos no começo do projeto através de inspeções de
mercado, entrevistas com usuários ou simplesmente suposições da equipe de
desenvolvimento. Valida também a interação entre os componentes do produto, como
por exemplo, a forma em que a documentação, a ajuda, o software e o hardware estão
integrados uns com os outros. Outro objetivo é prever o lançamento de um produto
novo no mercado que possivelmente necessite logo de manutenção.

O teste de validação enfatiza mais rigor experimental e de consistência desde
que seja dada importância a julgamentos quantitativos sobre o produto.

Teste de Comparação
O teste de comparação não é associado a nenhum ponto específico do ciclo de
desenvolvimento de um produto. Nos primeiros estágios, pode ser usado, para comparar
diferenças entre estilos de interface através do teste de exploração; nos ciclos
intermediários, pode ser usado para medir a efetividade de um elemento integrante da
interface; no final do ciclo, um teste de comparação pode ser usado para ve r como a
liberação de um produto atinge um produto concorrente.
O teste de comparação pode ser usado como uma junção dos demais testes sendo
que seu objetivo é realização de comparações em todos os níveis.


Preditiva - Tenta prever - Ex.: Avaliação Heurística
Interpretativa - Interpretação e observação - Ex.: Observação de Campo
Experimental - Ambientes controlados - Ex.: Testes de Usabilidade

Dados que o Teste de Usabilidade pode encontrar
Qualitativo
Opiniões
Relatos
Sugestões execução
Sugestões
Críticas
Satisfação
Quantitativo
Sugestões execução
No de erros
Tempo de execução
Tempo de finalização

Exemplo de Teste de Usabilidade em Protótipo de Papel
http://youtu.be/9wQkLthhHKA
Recomendações Básicas de Usabilidade
Bastien e Scapin - Necessário revisão
O sistema deve apresentar meios para orientar o usuário
O sistema deve retornar respostas ao usuários para cada ação, seja ela grande, pequena ou um conjunto de ações;
As respostas devem ser significativas, apropriadas para cada situação e em tempo razoável;
O sistema deve informar ao usuário o que está ocorrendo com ele. (status do sistema);
Deve fornecer meios para o usuário se localizar no sistema;
Deve fornecer ajuda para utilização do proprio sistema e suas ferramentas;
O sistema deve oferecer indicações de como o usuário deve proceder;
O sistema deve apresentar as informações de forma organizada (localização, caracteristicas gráficas, ondem alfabética, frequência de uso, etc...);

Deve diminuir a sobrecarga mental do usuário
A interface não deve sobrecarregar a visão do usuário com número elevado de informações, assim como informações irrelevantes ou pouco necessárias;
Se o canal visual estiver ocupado, podemos empregar o canal de áudio, sem sobrecarregá-los;
As tarefas devem ser simples, reduzindo o número de passos para realizá-las;
Todas as infromações presentes no sistema devem ser visíveis, respeitando característcias textuais comco cor, brilho, contraste, tamanho de corpo e espaçamentos;
Todas as informações devem ser claras e objetivas;
A interface deve ser projetada de dorma que a maneira de utilização do sistema seja explícita;
Deve priorizar as caracteristicas mais relevantes ao projetar a interface;

O usuário deve ter controle sobre o sistema
A velocidade de uso do sistema deve ser controlada pelo usuário;
Se possível, o sistema deve oferecer ações de desfazer (Ctrl + Z);
O sistema não deve executar ações que o usuário não tenha solicitado;
Se possível, o sistema deve fornecer ajustes e personalização das interfaces;

O sistema deve ser compatível e adaptável ao usuário
O sistema deve estar de acordo com com o nível de instrução, faixa etária, limitações do usuário e formas de utilização normalmente aceita.
O sistema deve utilizar termos familiares aos usuários, inclusive idioma, exceto termos já adotados pela língua;
O sistema deve ser flexível para atender diferentes níveis de experiência dos usuários, principiantes e experientes;
O sistema deve ser fornecer alternativas para usuários experientes ocultem informações destinadas aos usuários principiantes;
Se possível, o sistema deve fornecer ajustes e personalização das interfaces;
O sistema deve oferecer meios diferentes para se alcançar o mesmo objetivo;

O sistema deve evitar os erros e se ocorrerem, deve favorecer a sua correção
A interface deve ser projetada de maneira a evitar a ocorrência de erros circunstanciais propícias aos erros;
Para prevenir erros, o sistema pode solicitar as informações por etapas;
Se possível, o sistema deve oferecer ações de desfazer (Ctrl + Z)
O sistema deve solicitar a confirmação do usuário para ações irreversíveis;
Quando ocorre, os erros devem ser apresentados ao usuário com uma linguagem de fácil entendimento;
Os erros devem ser recuperados de maneira rápida e fácil;
O sistema deve fornecer meios para que o usuário corrija somente a parte incorreta;
As mensagem de erro devem ser claras e objetivas, utilizando vocabulário neutro. Não devem reprovar ou julgar o usuário;

O sistema deve utilizar padronização
A identidade visual deve ser respeitada em todo o sistema;
Deve existir padronização de localização dos elementos do sistema;
Deve existir padronização na forma como são realizadas as tarefas;
Deve existir padronização de termos utilizados no sistema;


Recomendações para Interface
Necessário revisão
Tente um layout com uma única coluna ao invés de múltiplas colunas.
Um layout de uma coluna vai dar mais controle sobre sua narrativa.
Foca o usuário no conteúdo.
Tente dar um presente ao invés de tentar fechar negócio logo de cara.
Um gesto amigável, como fornecer um presente como um e-book ou mesmo um obrigado, por exemplo, pode ser interessante. Presentear é uma tática de persuasão eficaz, que é baseado na regra da reciprocidade. Por mais óbvio que pareça, sendo bom para alguém através da oferta ou de um pequeno gesto de agradecimento pode encantar o usuário.
Tente agrupar funções similares ao invés de fragmentar a UI.
Isso diminui a curva de aprendizado do sistema. Avalie constantemente o sistema e considere refatorar seu UI de vez em quando , fundindo ações, botões, links e linguagens semelhantes. Lembrando que não existe mudança de layout pequena. Em cima de cada pequena ação é necessário um grande estudo para resolução do problema.
Tente fazer seus argumentos virem de outras pessoas, ao invés de falar de você mesmo.
Tente repetir o seu call-to-action ao invés de mostrar uma única vez.
Tente distinguir o que é clicável e selecionável do que não é.
Tente recomendar ao invés de mostrar várias opções com o mesmo peso.
“Nós achamos que essa opção é a melhora para você, mas fique livre para fazer sua escolha”.
Tente deixar o usuário desfazer, ao invés de pedir confirmação para tudo.
Tente focar em um público principal, ao invés de tentar agradar a todos.
Tente ser direto ao invés de ser indeciso.
Tente mostrar onde seu produto é feito, ao invés de deixa-lo genérico.
Tente menos campos de formulários, ao invés de querer pedir tudo de uma vez.
Tente mostrar as opções, ao invés de escondê-las.
Tente sugerir que há rolagem na página ao invés de deixar ela escondida.
Tente manter o foco ao invés de afogar o usuário em links.
Mostrar o estado em que o sistema ou item do sistema se encontra.
Os e-mails podem ser lidos ou não, as faturas podem ser pagas ou não, um item de uma tabela pode ser editado, excluido e etc. Informar os usuários sobre o estado particular em que um item está, é uma boa forma de fornecer feedback. Os estados em que eles se encontram podem ajudar as pessoas a entender as ações que foram realizados com sucesso ou se necessita de outra ação.
Ofereça vantagens ao invés de oferecer apenas tarefas nos botões.
Clique e baixe o livro. Clique aqui e economize.
Tente a manipulação direta a de utilizar menus específicos para ação.
Ao exibir listas de dados, por exemplo, podemos permitir que o usuário faça algo com os itens. Clicando ou passando o mouse por cima, ações como exluir, alterar, adicionar podem aparecer, permitindo que o item seja manipulado.
Tente animações ao apresentar itens ocultos.
Pode ser mais interessante apresentar um menu off-canvas vindo de uma animação do que simplesmente ele aparecer na tela.
Tente consistência ao invés de forçar o usuário aprender algo que ele não precisa.
Tente mostrar o status de preenchimento de formulários em tempo real.
Se por ventura o usuário esquecer de um campo ou preencher ele de forma errada, apresente isso em tempo real. Não espere que ele clique em enviar para avisa-lo que tem algum problema.
Apresente hierarquia visual.
Tente reconhecimento ao invés de recordação.
Grandes áreas para clicar.
Carregamento rápido!
Ícones acompanhados de nomes (label).
Utilize uma linguagem natural.

#Heurísticas de Nielsen

**Feedback
-O sistema deve informar continuamente ao usuário sobre o que ele está fazendo.
-10 segundos é o limite para manter a atenção do usuário focalizada no diálogo.

**Falar a linguagem do usuário
-A terminologia deve ser baseada na linguagem do usuário e não orientada ao sistema. As informações devem ser organizadas conforme o modelo mental do usuário.

**Saídas claramente demarcadas
-O usuário controla o sistema, ele pode, a qualquer momento, abortar uma tarefa, ou desfazer uma operação e retornar ao estado anterior.

**Consistência
-Um mesmo comando ou ação deve ter sempre o mesmo efeito.
-A mesma operação deve ser apresentada na mesma localização e deve ser formatada/apresentada da mesma maneira para facilitar o reconhecimento.

**Prevenir erros
-Evitar situações de erro.
-Conhecer as situações que mais provocam erros e modificar a interface para que estes erros não ocorram.

**Minimizar a sobrecarga de memória do usuário
-O sistema deve mostrar os elementos de diálogo e permitir que o usuário faça suas escolhas, sem a necessidade de lembrar um comando específico.

**Atalhos
-Para usuários experientes executarem as operações mais rapidamente.
-Abreviações, teclas de função, duplo clique no mouse, função de volta em sistemas hipertexto.
-Atalhos também servem para recuperar informações que estão numa profundidade na árvore navegacional a partir da interface principal.

**Diálogos simples e naturais
-Deve-se apresentar exatamente a informação que o usuário precisa no momento, nem mais nem menos.
-A seqüência da interação e o acesso aos objetos e operações devem ser compatíveis com o modo pelo qual o usuário realiza suas tarefas.

**Boas mensagens de erro
-Linguagem clara e sem códigos.
-Devem ajudar o usuário a entender e resolver o problema.
-Não devem culpar ou intimidar o usuário.

**Ajuda e documentação
-O ideal é que um software seja tão fácil de usar (intuitivo) que não necessite de ajuda ou documentação.
-Se for necessária a ajuda deve estar facilmente acessível on-line.

#Sessão de Avaliação

1. Visibilidade do status do sistema (Feedback)
Verificação: Os usuários são mantidos informados sobre o progresso do sistema com apropriado feedback em um tempo razoável?
Problema: _________________________________________________________________________________
Grau de severidade
(  ) Irrelevante - 0
(  ) Sem muita importância - 1
(  ) Baixa prioridade - 2
(  ) Grave - 3
(  ) Muito grave- 4

2. Compatibilidade entre o sistema e o mundo real
Verificação: O sistema utiliza conceitos e linguagem familiar com o usuário em vez de termos orientados ao sistema? O sistema utiliza convenções do mundo real, exibindo informações com uma ordem lógica e natural?
Problema: _________________________________________________________________________________
Grau de severidade
(  ) Irrelevante - 0
(  ) Sem muita importância - 1
(  ) Baixa prioridade - 2
(  ) Grave - 3
(  ) Muito grave- 4

3. Liberdade e controle do usuário
Verificação:
Os usuários podem fazer o que querem quando querem?
Problema:
Grau de severidade
(  ) Irrelevante - 0
(  ) Sem muita importância - 1
(  ) Baixa prioridade - 2
(  ) Grave - 3
(  ) Muito grave- 4

4. Consistência e padrões
Verificação: O projeto de elementos como objetos e ações tem o mesmo significado ou efeito em diferentes situações?
Problema: _________________________________________________________________________________
Grau de severidade
(  ) Irrelevante - 0
(  ) Sem muita importância - 1
(  ) Baixa prioridade - 2
(  ) Grave - 3
(  ) Muito grave- 4

5. Prevenção contra erros
Verificação: Os usuários podem cometer erros dos quais bons projetos poderiam prevenir?
Problema: _________________________________________________________________________________
Grau de severidade
(  ) Irrelevante - 0
(  ) Sem muita importância - 1
(  ) Baixa prioridade - 2
(  ) Grave - 3
(  ) Muito grave- 4

6. Reconhecimento em lugar de lembrança
Verificação: Os elementos de projeto como objetos, ações e opções são possíveis? O usuário é forçado a relembrar informações de uma parte do sistema para outra?
Problema: _________________________________________________________________________________
Grau de severidade
(  ) Irrelevante - 0
(  ) Sem muita importância - 1
(  ) Baixa prioridade - 2
(  ) Grave - 3
(  ) Muito grave- 4

7. Flexibilidade e eficiência de uso
Verificação: As tarefas são eficientes e podem se adaptar ao gosto do usuário em suas ações mais freqüentes? Os usuários podem utilizar teclas de atalho, macros e navegação simples que facilitam e agilizam a interação?
Problema: _________________________________________________________________________________
Grau de severidade
(  ) Irrelevante - 0
(  ) Sem muita importância - 1
(  ) Baixa prioridade - 2
(  ) Grave - 3
(  ) Muito grave- 4

8. Projeto minimalista e estético
Verificação: Os diálogos contém informações irrelevantes ou raramente necessárias?
Problema:_________________________________________________________________________________
Grau de severidade
(  ) Irrelevante - 0
(  ) Sem muita importância - 1
(  ) Baixa prioridade - 2
(  ) Grave - 3
(  ) Muito grave- 4
9. Auxiliar os usuários a reconhecer, diagnosticar e recuperar-se de erros


Verificação:

As mensagens de erro são expressas em linguagem simples (sem códigos) descrevendo exatamente o problema e sugerindo uma solução?
Problema: _________________________________________________________________________________
Grau de severidade
(  ) Irrelevante - 0
(  ) Sem muita importância - 1
(  ) Baixa prioridade - 2
(  ) Grave - 3
(  ) Muito grave- 4

10. Ajuda e documentação
Verificação: São fornecidas apropriadas informações de ajuda, e estas informações são fáceis de procurar e de focalizar nas tarefas do usuário?
Problema: _________________________________________________________________________________
Grau de severidade
(  ) Irrelevante - 0
(  ) Sem muita importância - 1
(  ) Baixa prioridade - 2
(  ) Grave - 3
(  ) Muito grave- 4


11. Diálogos que indicam término de ação
Verificação: As seqüências de ações do sistema deve são organizada? O usuário consigue entender os passos e sabe quando cada um deles acaba?

Problema: _________________________________________________________________________________
Grau de severidade
(  ) Irrelevante - 0
(  ) Sem muita importância - 1
(  ) Baixa prioridade - 2
(  ) Grave - 3
(  ) Muito grave- 4


Questionário de Satisfação
Obrigado por responder ao nosso questionário de satisfação. O questionário demora apenas 5 minutos do seu tempo.

Por favor aponte o seu nível de satisfação com uma das seguintes opções:
1 = Concordo Plenamente 	   2 = Discordo Plenamente		3 = Concordo em Partes

[   ] Esse site é interessante para mim
[   ] Você conseguiu achar o produto facilmente
[   ] O site tem produtos que me interessa
[   ] Eu me senti à vontade comprando no site

Sobre a aparência do site:
[   ] bonita		
[   ] feia
[   ] agradável    	        	
[   ] sem graça         	   
[   ] descontraída          	
[   ] chata
[   ] divertida		
[   ] séria

Sobre o carregamento do website:
[   ] muito rápido       	  
[   ] rápido		
[   ] lento	         	
[   ] muito lento

Sobre o uso do website:
[   ] divertida	 	  
[   ] descontraída	
[   ] séria 	                
[   ] chata      
 
Com que frequência você acha que realizará compras em nosso site?
[   ] toda semana          
[   ] todo mês          
[   ] de vez em quando          
[   ] raramente          
[   ] nunca

Em qual parte do processo da compra dos produtos você teve mais dificuldade?
____________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________

Acha que faltou algo? Quer dar alguma sugestão? 
____________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________

Caso ache necessário, adicionar mais perguntas.

#Artigos
Estudo da HUGE sobre scrolling: Everybody Scrolls
As implicações do campo de busca na experiência do usuário
Os problemas de design do novo padrão de navegação da Globo.com

#Ferramentas
Lista de afazares para UX: UX Project Checklist
Calcular tamanho dos Títulos e Textos: Type Scale
Lista de ferramentas para Web Designers: Best Tolls for Designers

#Frameworks CSS
Bootstrap
Foundation
Pure.io
UIKit
Material Design

#Ferramentas WordPress
Criação de todo tipo de custom types: Generate WP
Ícones do WordPress: Dashicons
Para adicionar esses ícones no menu administrativo, basta, ao cria o custom post type, adicionar logo a baixo da posição dele no menu 'menu_icon' => 'nome-do-icone'. Ex: 'menu_icon' => 'dashicons-admin-comments'


#Sugestões
Criar um blank theme do WordPress para gente (Feito - Trantor)
Criar um framework próprio que atenda nossas necessidades... Ou modificar um
