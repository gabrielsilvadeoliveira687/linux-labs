# 01 - INTRODUÇÃO: CONCEITOS, DISTRIBUIÇÕES E HISTÓRICO DO LINUX

## INTRODUÇÃO AO LINUX

**O Linux é um dos sistemas operacionais mais utilizados e respeitados no mundo da tecnologia**, conhecido por sua estabilidade, flexibilidade e natureza de código aberto. Ele é amplamente adotado em servidores, desktops e em todos os principais provedores de serviços de nuvem. Este material oferece uma visão geral do Linux, abordando seus conceitos fundamentais, histórico, vantagens, componentes essenciais e aspectos necessários para utilizá-lo de forma eficiente.

## HISTÓRICO

**O Linux foi criado em 1991 por Linus Torvalds**, estudante de pós-graduação na Universidade de Helsinque, Finlândia. Ele se inspira no Unix, um sistema operacional desenvolvido no final dos anos 1960, mas com o diferencial de ser totalmente de código aberto. A arquitetura modular do Linux permite extensões e customizações, tornando-o adequado tanto para desktops quanto para servidores. Além disso, sua estabilidade reduz a necessidade de reinicializações frequentes, evitando travamentos comuns em outros sistemas.

## ESTRUTURA DE DIRETÓRIOS

**O Linux organiza seus arquivos em uma hierarquia clara, baseada no diretório raiz (`/`)**. Abaixo estão alguns dos diretórios principais e suas funções:

- **/bin**: Contém comandos essenciais do sistema, como `ls`, `rm`, `pwd`, `cat` e `su`.  
- **/boot**: Armazena arquivos necessários para a inicialização do sistema.  
- **/dev**: Inclui arquivos de dispositivos, representando componentes de hardware como HDs, CD-ROMs e outros dispositivos conectados.  
- **/etc**: Diretório de configuração do sistema, similar ao “registro” do Windows.  
- **/home**: Pastas pessoais dos usuários. Cada usuário possui seu próprio subdiretório, e apenas arquivos dentro dele podem ser modificados por usuários comuns.  
- **/lib**: Bibliotecas essenciais para o funcionamento do sistema e programas. Existem bibliotecas compartilhadas (`.so`) e específicas (`.a`).  
- **/mnt e /media**: Pontos de montagem de dispositivos externos, como pen drives ou discos adicionais.  
- **/proc**: Informações dinâmicas sobre processos e o Kernel.  
- **/sbin**: Ferramentas administrativas do sistema, geralmente acessíveis apenas pelo usuário root.  
- **/tmp**: Armazena arquivos temporários utilizados por programas e pelo sistema.  
- **/usr**: Contém a maior parte dos programas e utilitários do sistema, incluindo `/usr/bin`, onde se encontram milhares de aplicativos.  
- **/var**: Guarda dados que mudam frequentemente, como logs, caches e bancos de dados temporários.

## O DIRETÓRIO HOME

**Cada usuário possui uma pasta pessoal chamada HOME**. A variável `$HOME` aponta para o diretório do usuário atual, e o símbolo `~` também representa o mesmo caminho. É dentro desta pasta que usuários comuns podem criar, modificar e armazenar seus arquivos sem afetar outros usuários ou o sistema.

## NAVEGAÇÃO E ARQUIVOS

**No Linux, tudo é tratado como um arquivo** — documentos, diretórios, dispositivos e até processos. Isso proporciona grande flexibilidade e permite que ferramentas comuns sejam usadas de forma consistente em diferentes tipos de arquivos.  

Por exemplo, é possível listar processos como se fossem arquivos utilizando o comando:

```bash
ls /proc
