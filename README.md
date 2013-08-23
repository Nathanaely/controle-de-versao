controle-de-versao
==================

trabalho de II

Histótia :
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


Vantagens e desvantagens :


Controle de versão distribuído (Distributed Version Control Systems – DVCS) 
é a mais nova geração de sistemas de controle de versão de software. 
Apesar de o conceito existir já há algum tempo, recentemente as ferramentas se tornaram maduras 
o suficiente para chamar a atenção de diversos projetos open source, que migraram ou expandiram 
seu suporte do Subversion (centralizado) para o Mercurial, Git e Bazaar (distribuídos) por exemplo.

Mas o que tem de errado com o controle de versão centralizado? Nada. 
Ele usa uma estrutura que atende muito bem a grande parte das equipes de desenvolvimento de software. 
Baseia-se na arquitetura cliente-servidor, com um repositório central (servidor) e cópias de trabalho 
para os desenvolvedores (clientes).

Para equipes de desenvolvimento com acesso ao repositório pela rede local, 
essa arquitetura funciona bem. A velocidade da rede não é problemática, 
o tempo de resposta do processamento é aceitável e todos os desenvolvedores da 
equipe têm permissão de leitura e escrita no repositório.

Não foi para resolver exatamente esse tipo de necessidade que o controle de versão 
distribuído foi criado. Imagine uma situação diferente:

Equipe com centenas de desenvolvedores. Significa que mais processamento vai ser exigido do servidor central, 
piorando o tempo de resposta;
Equipe espalhada em diferentes filiais da empresa.
Acesso remoto ao repositório com limitações de conexão e de permissão de escrita;
A arquitetura cliente-servidor não funciona tão bem para essas situações. 
Soluções alternativas como aumentar a capacidade de processamento do 
servidor ou replicar os repositórios nem sempre são viáveis ou fáceis de serem implementadas.

Para essas situações, a arquitetura peer-to-peer, na qual o controle de versão distribuído se baseia, 
é muito mais adequada.

Benefícios do Controle de Versão Distribuído

As vantagens estão relacionadas à distribuição do processamento, 
redundância/replicação de repositórios e as novas possibilidades de colaboração entre desenvolvedores.

Resumo das Características do Controle de Versão Distribuído

Ponto de Vista	Vantagens	Desvantagens
Desenvolvedor	
Rapidez
Autonomia
Ramos Privados
Facilidade de Mesclagem
Necessidade de maior conhecimento da ferramenta e do processo
Coordenação/Gerência	
Redução de custos com servidor e infraestrutura externa de rede
Confiabilidade
Aumento da produtividade
Necessidade de maior capacitação de desenvolvedores
Importante ter um processo definido
O controle de mudança ainda precisa ser centralizado
Considerações Finais

Controle de versão distribuído oferece muitas vantagens interessantes. 
Mesmo projetos que não se encaixam diretamente no perfil podem se beneficiar. 
Entretanto, por ser um pouco mais complexo, o modelo distribuído requer mais preparo da equipe e também do processo, 
o que não chega a ser realmente um impedimento uma vez que um processo formalizado e 
equipes capacitadas são fundamentais para produção de software de qualidade.

Em um próximo artigo, vou analisar alguns pontos que ajudarão a decidir a viabilidade ou não de 
se mudar do centralizado para o controle de versão distribuído.
