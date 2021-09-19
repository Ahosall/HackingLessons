# Metasploit

Metasploit é um projeto de segurança de informação que divulga informações relacionadas a vulnerabilidades e busca facilitar testes de penetração e o desenvolvimento de Sistema de detecção de intrusos. O projeto pertence a empresa Rapid7. 

## O que é Metasploit?

Metasploit é um projeto de segurança de informação que divulga informações relacionadas a vulnerabilidades ("exploits") e busca facilitar testes de penetração ("pentests") e o desenvolvimento de Sistema de detecção de intrusos.

## Qual o novo banco de dados que o Metasploit 5 usa?

A nova versão moderniza a forma como o Metasploit interage com dados e outras ferramentas. Com o banco de dados Postgresql por exemplo, adiciona a capacidade de executar o banco de dados sozinho como um serviço RESTful, com o qual vários consoles Metasploit e até mesmo ferramentas externas podem interagir.

Qual é o comando utilizado para configurar o endereço remoto no alvo dentro do Metasploit?

No nosso caso, usaremos o tcp meterpreter, o qual gera um shell remoto no servidor, quando o ataque obtêm êxito.

## Como funciona?

O teste de penetração é hackeando com permissão. Você deve ter visto hackers legais na TV atacando sistemas de computador sem serem pegos. Mas não é assim que funciona no mundo real.

Se você hackear alguém sem permissão, há uma grande chance de você acabar na prisão. Portanto, se você está planejando aprender a hackear com más intenções, não sou responsável por nenhum dano que você causar. Todos os meus artigos são puramente educacionais.

Então, se hackear é ruim, por que aprender isso em primeiro lugar? Cada dispositivo na Internet é vulnerável por padrão, a menos que alguém o proteja.

Recentemente, escrevi um artigo sobre as dez principais ferramentas que você deve conhecer como engenheiro de segurança cibernética. Se você estiver interessado em aprender mais sobre segurança cibernética, Confira o artigo aqui.

Certo. Chega de conversa estimulante. Vamos dar uma olhada em uma das ferramentas de teste de caneta mais legais do mercado – Metasploit.
Isso inclui reconhecimento, varredura, exploração, escalonamento de privilégios e manutenção de acesso.

Metasploit é uma estrutura de código aberto escrita em Ruby. Ele foi escrito para ser uma estrutura extensível, de modo que, se você deseja construir recursos personalizados usando Ruby, você pode fazer isso facilmente por meio de plug-ins.

Rapid7, a empresa por trás da Metasploit, oferece um versão premium do Metasploit com recursos avançados.

Metasploit também é frequentemente atualizado com novos exploits publicados no Vulnerabilidades e exposições comuns (CVE). Portanto, se uma nova vulnerabilidade for encontrada e publicada, você pode começar a verificar seus sistemas imediatamente.

Metasploit vem com ferramentas anti-forenses e evasão integradas a ele. Também é pré-instalado no Sistema operacional Kali.

Agora que você sabe o que é o Metasploit, vamos examinar os principais conceitos do Metasploit.

Metasploit oferece alguns componentes-chave para encontrar e explorar vulnerabilidades em uma rede. Isso inclui exploits, payloads, auxiliares e assim por diante. Vamos examinar cada um deles em detalhes.

## Exploits

Um exploit é um pedaço de código que tira proveito de uma vulnerabilidade em um sistema. Essas explorações executam ações específicas com base em quão ruim é a vulnerabilidade.

As explorações podem tirar proveito de vulnerabilidades de software, vulnerabilidades de hardware, vulnerabilidades de dia zero, e assim por diante. Algumas das explorações comuns incluem estouros de buffer, injeções de SQL e assim por diante.

Metasploit oferece uma série de exploits que você pode usar com base nas vulnerabilidades existentes no sistema de destino. Essas explorações podem ser classificadas em dois tipos:

Explorações ativas – Explorações ativas serão executadas em um sistema de destino, explorar o sistema, dar-lhe acesso ou executar uma tarefa específica e, em seguida, sair.

Exploits passivos – Os exploits passivos irão esperar até que o sistema de destino se conecte ao exploit. Essa abordagem é frequentemente usada por hackers na Internet que solicitam o download de arquivos ou software. Depois de fazer isso, você se conecta a um exploit passivo em execução no computador do hacker.

## Cargas Úteis

Uma carga útil é um trecho de código executado por meio do exploit. Você usa exploits para entrar em um sistema e cargas úteis para realizar ações específicas.

Por exemplo, você pode usar um keylogger como uma carga útil junto com um exploit. Assim que a exploração for bem-sucedida, ele instalará o keylogger no sistema do alvo.

Metasploit oferece uma boa coleção de cargas úteis, como shells reversos, shells de ligação, Meterpreter e assim por diante.

Existem alguns payloads que funcionarão com a maioria dos exploits, mas é necessária alguma pesquisa para encontrar o payload certo que funcionará com o exploit.

Depois de escolher um exploit, você pode listar os payloads que funcionarão com aquele exploit usando o comando ‘show payloads’ no Metasploit.

Existem alguns tipos de payloads no Metasploit. Os que você vai acabar usando mais são estes três tipos:

Músicas – Payloads que funcionam por conta própria, por exemplo, keyloggers.

Stagers – Cargas que funcionam com outras, por exemplo duas cargas: uma para estabelecer uma conexão com o alvo, outra para executar uma instrução.

Medidor – Carga útil avançada que reside na memória do destino, difícil de rastrear e pode carregar / descarregar plug-ins à vontade. Há uma seção abaixo sobre Meterpreter onde vou explicar em detalhes.

## Auxilares

Auxiliares são módulos que ajudam a executar funções personalizadas além da exploração de um sistema. Isso inclui scanners de porta, fuzzers, sniffers e muito mais.

Por exemplo, você pode usar o CERT auxiliar para verificar se há certificados SSL expirados em uma rede. Isso é útil para administradores de sistema para automatizar o gerenciamento de certificados.

Se você está familiarizado com Ruby, pode escrever seus próprios auxiliares. Se você deseja varrer uma rede em busca de vulnerabilidades específicas toda semana, pode escrever seu próprio módulo auxiliar personalizado para fazer isso.

Você pode então usá-lo para verificar sua rede em vez de usar um scanner existente como Nmap.

Agora que você sabe como funciona o Metasploit, vamos dar uma olhada nas ferramentas que o Metasploit oferece.

## MsfConsole

MsfConsole é a interface padrão do Metasploit. Ele fornece todos os comandos de que você precisa para interagir com o framework Metasploit.

Leva um pouco de curva de aprendizado para se familiarizar com a CLI, mas depois que você fizer isso, será fácil trabalhar com ela. Além disso, MsfConsole é a única maneira de acessar todos os recursos do Metasploit.

O MsfConsole também oferece preenchimento de tabulação para comandos comuns. Familiarizar-se com o MsfConsole é um passo importante em sua jornada para se tornar um profissional Metasploit.

## MsfDB

Se você trabalha com grandes redes regularmente, provavelmente precisará de um local para armazenar seus dados. Isso inclui resultados de varredura, credenciais de login e assim por diante.

Metasploit oferece uma ferramenta de gerenciamento de banco de dados chamada msfdb. msfdb funciona em cima de um banco de dados PostgreSQL e fornece uma lista de comandos úteis para importar e exportar seus resultados.

Com o msfdb, você pode importar os resultados da verificação de ferramentas externas como Nmap ou Nessus. Metasploit também oferece um comando nativo db_nmap que permite escanear e importar resultados usando Nmap dentro do msfconsole.

## MsfVenom

Finalmente, temos msfvenom (nome legal, hein?). msfvenom permite gerar cargas personalizadas, dependendo do seu destino.

Usar um antivírus ou firewall pode tornar um sistema de destino relativamente seguro. Nesses casos, os payloads Metasploit existentes podem não funcionar, pois são genéricos para todos os sistemas incluídos em um sistema operacional ou serviço.

msfvenom foi construído combinando duas ferramentas mais antigas que o Metsploit tinha: msfpayload e msfencode. msfvenom permite que você crie e codificar cargas úteis personalizadas para seus exploits.

Com base nas informações adicionais que você tem sobre o alvo, você pode criar suas próprias cargas úteis para obter uma taxa de sucesso mais alta durante o teste de penetração.

Meterpreter é uma carga útil avançada no Metasploit. Ao contrário de outras cargas úteis que executam uma função específica, o Meterpreter é dinâmico e pode ser programado imediatamente.

Se você pode explorar um sistema e injetar Meterpreter como carga útil, aqui estão algumas coisas que você pode fazer:

Estabeleça uma comunicação criptografada entre seu sistema e o destino.

Descarregue hashes de senha do sistema de destino.

Procure por arquivos no sistema de arquivos de destino

Carregar / baixar arquivos

Tire fotos da webcam

Meterpreter também é incrivelmente furtivo. Como o Meterpreter vive na memória do alvo, é extremamente difícil de detectar. Também é difícil rastrear o Meterpreter usando ferramentas forenses.

O principal recurso do Armitage é visualizar alvos e recomendar exploits. Armitage também pode ser programado por script, o que significa que você pode automatizar tarefas redundantes, como descoberta de host.

Armitage é extremamente útil quando você está trabalhando com um grande número de sistemas em uma rede. Você pode usar a GUI de Armitage para escalar privilégios, navegar por arquivos, despejar hashes de senha e assim por diante.

Metasploit fornece um conjunto de ferramentas para você realizar uma auditoria completa de segurança de uma rede. Metasploit é freqüentemente atualizado com as vulnerabilidades publicadas no banco de dados Common Vulnerabilities and Exploits.

Você também pode usar outras ferramentas como Nmap e Nessus com Metasploit por meio de integrações ou importando seus relatórios de varredura para Metasploit. Metasploit também possui uma ferramenta GUI chamada Armitage que permite visualizar alvos e recomendar exploits.

Se você estiver interessado em aprender mais sobre o Metasploit, verifique o guia de referência detalhado publicado pela Offensive Security.

---
<p align="center">
  Professor - <a href="https://github.com/SPAWN-cloud"><b>Spawn</b></a> - Para duvidas clique <a href="https://wa.me/5551982593521">Aqui</a>.
</p>