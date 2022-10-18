# Exercícios - agora, a prática

É hora de colocar a mão na massa. 💪🏼
⚠️ Lembre-se de manter sua pasta de exercício organizada.
Você já pode consultar o conteúdo sobre portfólio de exercícios para mais dicas de como organizá-lo.

Logo mais você vai aprender sobre o GitHub e poderá guardar seus exercícios em repositórios e montar seu portfolio profissional!


# Exercícios - comandos de input e output

# Requisitos: 

* Crie a pasta unix_tests_skills e navegue até ela.
* Crie um arquivo texto pelo terminal com o nome skills2.txt e adicione os valores Internet, Unix e Bash, um em cada linha.
* Adicione mais 5 itens à sua lista de skills e depois imprima a lista ordenada no terminal. 🤓
* Conte quantas linhas tem o arquivo skills2.txt.
* Crie um arquivo chamado top_skills.txt usando o skills2.txt, contendo as 3 primeiras skills em ordem alfabética.
* Crie um novo arquivo chamado phrases2.txt pelo terminal e adicione algumas frases de sua escolha.
* Conte o número de linhas que contêm as letras br.
* Conte o número de linhas que não contêm as letras br.
* Adicione dois nomes de países ao final do arquivo phrases2.txt.
* Crie um novo arquivo chamado bunch_of_things.txt com os conteúdos dos arquivos phrases2.txt e countries.txt
* Ordene o arquivo bunch_of_things.txt.


# Exercícios - permissões

# Requisitos: 

* Crie a pasta unix_tests_permissions e navegue até ela.
* Rode o comando ls -l e veja quais as permissões dos arquivos.
* Crie o arquivo arquivo_teste.txt.
* Mude a permissão do arquivo arquivo_teste.txt para que todas as pessoas usuárias possam ter acesso à leitura e escrita, e verifique se está correto com o comando ls -l;
* Resultado esperado: -rw-rw-rw- 1 ana ana 1860 ago 13 11:39 arquivo_teste.txt
* Tire a permissão de escrita do arquivo arquivo_teste.txt para todas as pessoas usuárias, verifique se está correto com o comando ls -l;
* Resultado esperado: -r--r--r-- 1 ana ana 1860 ago 13 11:39 arquivo_teste.txt
* Volte à permissão do arquivo arquivo_teste.txt para a listada inicialmente utilizando o comando chmod 644 arquivo_teste.txt.
* Resultado esperado: -rw-r--r-- 1 ana ana 1860 ago 13 11:39 arquivo_teste.txt


# Exercícios - processos & jobs

# Requisitos: 

* Liste todos os processos.
* Agora use o comando sleep 30 &.
* Use a listagem de processos para encontrar o PID do processo que está executando o comando sleep 30 e termine a sua execução ~~(mate o processo)~~.
* Execute novamente o comando sleep 30, mas agora sem o &. Depois, faça com que ele continue executando em background.
* Crie um processo em background que rode o comando sleep por 300 segundos.
* Crie mais dois processos que rodem o comando sleep por 200 e 100 segundos, respectivamente.
* Você deve criá-los em foreground (sem usar o &) e suspendê-los (apertando ctrl+z) após cada um começar a executar.
* Verifique que apenas o processo sleep 300 está em execução com o comando jobs. Suspenda a execução desse processo.
* Você vai precisar trazer o processo para foreground (fg) e suspendê-lo (ctrl+z), ou enviar um sinal.
* Retome a execução do processo sleep 100 em background com o comando bg.
* Termine a execução de todos os processos sleep ~~(mate os processos)~~.


# Exercícios - (bônus) - o despertar do terminal

E para terminar com a energia ~~óh,~~ lá no alto, que tal aprender agora alguns comandos divertidos do Unix? ☝ 🎊

Se você utiliza macOS, precisa ter o gerenciador de pacotes brew instalado. Para isso, siga as orientações neste link.

1- Após instalar o brew, instale o factor e o telnet:

2- Para instalar o factor, execute no terminal: brew install coreutils;

3- Para instalar o telnet, execute no terminal: brew install telnet.

# Requisitos: 

* Se você utiliza o Linux, abra o terminal e execute o comando sudo apt-get install cmatrix, ou para pessoas usuárias de macOS, utilize no terminal brew install cmatrix. Depois, execute o comando cmatrix. Quando estiver se sentindo como o Neo, aperte ctrl+c para voltar ao terminal;
* No sistema Linux, execute o comando sudo apt-get install fortune, ou no macOS brew install fortune e, após a instalação, crie um arquivo de texto chamado fortune.txt que contenha a sua sorte do dia. Utilize apenas uma linha de comando. Dica: use o comando fortune, e o operador >;
* Conte quantas palavras tem a frase da sua sorte do dia. Dica: use o comando wc;
* Execute o comando sudo apt-get install sl em um terminal Linux, ou brew install sl em um terminal macOS. Após a instalação, execute o comando sl. Agora tente sl -f;
* No sistema Linux, execute o comando sudo apt-get install cowsay, ou brew install cowsay no macOS. Após a instalação, execute o comando cowsay e algo que você queira falar. Agora faça a vaquinha dizer a frase que está gravada no arquivo fortune.txt;
* Descubra os fatores primos usando o comando factor e em seguida o número 42;
* Veja como fica a sua sorte do dia ao contrário. Dica: utilize o comando rev;
* Execute o comando telnet towel.blinkenlights.nl e espere alguns segundos. Lembre-se de que você tem mais exercícios para fazer! 😅

Gostou das curiosidades? Nos Recursos Adicionais tem mais alguns comandos divertidos. Confere lá!
