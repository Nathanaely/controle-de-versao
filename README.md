controle-de-versao
==================

trabalho de II

História :
Mercurial é uma ferramenta multi-plataforma de controle de versão distribuído para desenvolvedores de software. 
O sistema é implementado principalmente em Python, porém o utilitário binário diff foi escrito em C. 
Mercurial foi inicialmente escrito para rodar sobre Linux, mas foi portado para Windows, Mac OS X, 
e a maioria dos outros sistemas UNIX. Mercurial é principalmente um programa de linha de comando. 
Todas operações do Mercurial são chamadas através de palavras chave de opções para o programa controlador hg, 
uma referência para o símbolo químico do elemento Mercúrio.
A Weblibre usa o sistema de controle de versões Mercurial (http://mercurial.selenic.com). 
Trata-se de um sistema de fácil aprendizagem mas dotado das principais funcionalidades deste tipo de sistema.
No Mercurial, cada cópia de trabalho (working copy) é também um repositório completo, 
que pode ser usado para gerar outras cópias de trabalho ou resgatar versões anteriores.
Além disso, há uma ferramenta gráfica que auxilia em todas as tarefas relacionadas ao controle de versão. 
Trata-se do Tortoise HG (http://tortoisehg.bitbucket.org). Este utilitário é integrado ao Windows Explorer.
Como estavamos acostumados ao SVN, foi necessário fazer algumas configurações 
adicionais para que o Mercurial funcionasse de maneira parecida àquela que estavamos acostumados.


forma de criar um repositório:

Criando um Repositório

Crie um repositório com o comando hg init:

alice$ ls
alice$ hg init example
alice$ ls
example
O comando hg init criou um novo diretório que é o novo repositório. 
Poderíamos ter criados o diretório example e depois executado o comando hg init sem parâmetros
dentro desse diretório para torná-lo um repositório.

Entrando no diretório example pode-se observar:

alice$ cd example
alice$ ls -a
.
..
.hg
Como você pode ver, o novo diretório está vazio exceto por um diretório .
hg na raiz do diretório. O Mercurial armazena o histórico e outros arquivos administrativos neste diretório.

