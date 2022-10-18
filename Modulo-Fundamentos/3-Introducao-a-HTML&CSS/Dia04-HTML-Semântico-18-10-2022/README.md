A partir de agora, você sempre verá uma seção mostrando como realizar o versionamento do seu código antes da descrição dos exercícios do dia. Então, para te ajudar a organizar seus exercícios criamos um conteúdo focado nisso que está cheio de exemplos, você pode acessá-lo aqui.

No conteúdo que criamos, você será apresentado a uma estrutura de organização utilizando pastas para módulos e para seções. Essa estrutura é diferente da que você verá na seção de versionamento do código do conteúdo do dia, fica a seu critério decidir qual a melhor forma de organizar seus exercícios!

Caso haja alguma dúvida ou você queira dar um feedback sobre esse conteúdo, mande uma mensagem no Slack!

# Exercícios - antes de começar

# Versionando seu código
Para versionar seu código, utilize o seu repositório de exercícios. 😉

Abaixo você vai ver exemplos de como organizar os exercícios do dia em uma branch, com arquivos e commits específicos para cada exercício. Você deve seguir este padrão para realizar os exercícios a seguir.

1. Abra a pasta de exercícios:

cd ~/trybe-exercicios

2. Certifique-se de que está na branch main e ela está sincronizada com a remota. Caso você tenha arquivos modificados e não comitados, deverá fazer um commit ou checkout dos arquivos antes deste passo.

git checkout main
git pull

3. A partir da main, crie uma branch com o nome exercicios/<modulo>-<secao>.<dia>. Onde <modulo> representa o módulo <secao> representa a seção atual e <dia> representa o dia do conteúdo. Por exemplo exercicios/fundamentos-4.2.

git checkout -b exercicios/<modulo>-<secao>.<dia>

4. Caso seja o primeiro dia deste módulo, crie um diretório com o nome do módulo e o acesse na sequência:

mkdir <nome-do-módulo>
cd <nome-do-módulo>

5. Caso seja o primeiro dia da seção, crie um diretório para ela seguindo o padrão secao-<secao>-<título-da-secao>, onde <secao> representa o número da seção e <título-da-secao> representa o título do conteúdo da seção. Por exemplo: secao-4-introducao-a-javascript-e-logica-de-programacao. Depois de criar o diretório, acesse-o usando o comando cd.

mkdir secao-<secao>-<título-da-secao>
cd secao-<secao>-<título-da-secao>

6. Crie um diretório para o dia seguindo o padrão dia-<dia>-<título-do-dia>, onde <dia> representa o número do dia e <título-do-dia> representa o título do conteúdo do dia. Por exemplo: dia-2-javascript-array-e-loop-for. Depois de criar o diretório, acesse-o usando o comando cd.

mkdir dia-<dia>-<título-do-dia>
cd dia-<dia>-<título-do-dia>

7. Os arquivos referentes aos exercícios deste dia deverão ficar dentro do diretório ~/trybe-exercicios/<nome-do-módulo>/secao-<secao>-<título-da-secao>/dia-<dia>-<título-do-dia>. Lembre-se de fazer commits pequenos e com mensagens bem descritivas, preferencialmente a cada exercício resolvido.

Verifique os arquivos alterados/adicionados:

git status
On branch exercicios/<modulo>-<secao>.<dia>
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

  modified:   exercicio-1

  Adicione os arquivos que farão parte daquele commit:

  # Se quiser adicionar os arquivos individualmente
git add <caminho-para-o-arquivo>

# Você também pode adicionar todos os arquivos de uma vez, porém, atente-se para não adicionar arquivos indesejados acidentalmente
git add --all

Faça o commit com uma mensagem descritiva das alterações:

git commit -m "Mensagem descrevendo alterações"

8. Você pode visualizar o log de todos os commits já feitos naquela branch com git log.

git log
commit 100c5ca0d64e2b8649f48edf3be13588a77b8fa4 (HEAD -> exercicios/<modulo>-<secao>.<dia>)
Author: Tryber Bot <tryberbot@betrybe.com>
Date:   Wed Feb 09 17:48:01 2022 -0300

    Exercicio 2 - mudando o evento de click para mouseover, tirei o alert e coloquei pra quando clicar aparecer uma imagem do lado direito da tela

commit c0701d91274c2ac8a29b9a7fbe4302accacf3c78
Author: Tryber Bot <tryberbot@betrybe.com>
Date:   Wed Feb 09 16:47:21 2022 -0300

    Exercicio 2 - adicionando um alert, usando função e o evento click

commit 6835287c44e9ac9cdd459003a7a6b1b1a7700157
Author: Tryber Bot <tryberbot@betrybe.com>
Date:   Wed Feb 09 15:46:32 2022 -0300

    Resolvendo o exercício 1 usando eventListener

9. Agora que temos as alterações salvas no repositório local precisamos enviá-las para o repositório remoto. No primeiro envio, a branch exercicios/<modulo>-<secao>.<dia> não vai existir no repositório remoto, então precisamos configurar o remote utilizando a opção --set-upstream (ou -u, que é a forma abreviada).

git push -u origin exercicios/<modulo>-<secao>.<dia>

10. Após realizar o passo 9, podemos abrir a Pull Request a partir do link que aparecerá na mensagem do push no terminal, ou na página do seu repositório de exercícios no GitHub através de um botão que aparecerá na interface. Escolha a forma que preferir e abra a Pull Request. De agora em diante, você repetirá o fluxo a partir do passo 7 para cada exercício adicionado, porém como já definimos a branch remota com -u anteriormente, agora podemos simplificar os comandos para:

# Quando quiser enviar para o repositório remoto
git push

# Caso você queria sincronizar com o remoto, poderá utilizar apenas
git pull

11. Quando terminar os exercícios, seus códigos devem estar todos commitados na branch exercicios/<modulo>-<secao>.<dia>, e disponíveis no repositório remoto do GitHub. Pra finalizar, compartilhe o link da Pull Request no canal de Code Review para a monitoria e/ou colegas revisarem. Faça review você também, lembre-se que é muito importante para o seu desenvolvimento ler o código de outras pessoas. 🤜🏼🤛🏼



# xercícios - agora, a prática
Antes de fazer os exercícios, crie um arquivo HTML introducao-a-html-e-css e copie o código abaixo:

index.html

<!DOCTYPE html>
<html>
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width" />
  </head>
  <body>
    <!--insira os elementos aqui-->
  </body>
</html>

O objetivo desses exercícios é colocar em prática o que você aprendeu sobre HTML semântico.

Para tal, criaremos uma página que apresenta um dos animais mais impressionantes que existem: o Stomatopoda. A estilização da página fica a seu critério. 😉

Para uma melhor organização, faça commits a cada tarefa concluída. Vamos aos exercícios:

# Requisitos: 

* Adicione um cabeçalho na página contendo o título Soco a 80km/h: Conheça o Stomatopoda.
* Adicione um conjunto de links que representam a área de navegação do site.
* Crie um link chamado Página Inicial.
* Crie um link chamado Sobre.
* Crie um link chamado Contato.
* Crie um artigo que vai conter os fatos interessantes sobre o Stomatopoda. O artigo terá o subtítulo Fatos sobre o Stomatopoda. Segue um site animal de inspiração para pegar fatos.
D* ivida o artigo em seções, organizando-o da seguinte forma:
* Uma primeira seção contendo informações gerais a respeito do animal. O subtítulo para essa seção fica a seu critério. É necessário que conste nessa seção seu nome científico, que é Odontodactylus scyllarus, em itálico. Além disso, é preciso que haja informação tabular a respeito de sua classificação científica, em específico: Reino, Filo, Subfilo, Classe, Subclasse e Ordem. Tais informações você consegue obter na Wikipedia.
* As outras seções dizem respeito aos fatos interessantes que você escolheu acerca do animal. Para cada fato escolhido você vai criar uma seção.
* Adicione, para cada seção, um subtítulo referente ao fato escolhido.
* Adicione, para cada seção, parágrafo(s) descrevendo o fato escolhido. Destaque características impressionantes referentes ao fato que você escolheu, de forma a reforçar a unicidade do Stomatopoda. Por exemplo: se você criar uma seção detalhando o soco potente do animal, seria interessante destacar a velocidade desse soco (80km/h) em negrito.
* Adicione, para cada seção, uma imagem, como forma de ilustrar o fato.
* Adicione, por fim, uma seção de referências bibliográficas, contendo uma lista de todos os links que foram usados como base para compilar a página em questão.
* Adicione um conteúdo adjacente ao artigo, disponibilizando um link para este vídeo que mostra o animal em ação.
* Adicione um rodapé na página, mostrando algo do gênero:

"Conteúdo compilado por <insere seu nome>, <ano atual>".

Obs: para esse exercício, é obrigatório fazer uso de, no mínimo, 6 elementos com as seguintes tags: header, nav, article, section, h1, h2, h3, aside, footer, table e img.

# Validando com CodeSniffer

Tendo feito uma página HTML, suponha que uma pessoa com deficiência visual acesse sua página. Será que sua página estará acessível para essa pessoa? 🤔

Vamos averiguar!

Entre neste site , que valida se sua página é acessível ou não. Para isso, você deverá copiar o código HTML e colar na caixa em baixo de “Run your code through the Sniffer”.

Ao submeter o código, você vai se deparar com erros de validação presentes em sua página, agora como exercício: conserte todos os erros apontados.

Para cada erro de validação mostrado, você tem à disposição um link para a página com sua descrição. Antes de voltar para o código e já ir consertando, leia a descrição de cada erro para entendê-lo e poder consertá-lo.

No fim do exercício, além de ter uma página acessível, você vai reforçar a prática de consertar erros, seja de validação (para este exercício), seja de lógica, com que você vai se deparar ao longo de sua carreira de desenvolvedor.

# Validando com Lighthouse

Podemos usar o Lighthouse para verificar a acessibilidade e outras coisas. Para isto, abra o site que criou utilizando a extensão Live Server do VSCode. Iremos utilizar o DevTools do navegador Chrome para analisar a acessibilidade, seguindo os seguintes passos:

1. Abra o DevTools utilizando uma das seguintes formas: (OBS: Você deverá estar na janela do navegador)

* Aperte a tecla F12;
* Utilize o atalho CTRL + SHIFT + I;
* Através da interface clique nos três pontos na parte superior direita da tela, abrirá um menu, clique em More tools e depois em Developer Tools.

2. No menu superior haverão várias abas, a que queremos se chama Lighthouse. Caso ela esteja escondida, procure por um botão com o ícone similar a >>.

* Antes de selecionar: Elements
* Depois de selecionar: Lighthouse

3. Ao fazer isso aparecerá um painel onde é possível escolher o que queremos testar e gerar o relatório.

* Botão para gerar relatório: Generate report
* Seleção de categorias: Accessibility

4. Através do relatório podemos corrigir os problemas

* Relatório: http://127.0.0.1:5500/text.html
* Exemplo de erro de acessibilidade: Document doesn't have a <title> element
