
# 03 - COMANDOS BÁSICOS DO LINUX

## INTRODUÇÃO

**Esta seção apresenta uma lista dos principais comandos básicos do Linux**, essenciais para navegação, manipulação de arquivos, gerenciamento de usuários e processos, além de operação geral do sistema. É indicada para iniciantes que desejam se familiarizar com o terminal Linux.

## ABRINDO O PROMPT

- **Abrir o terminal no Linux:** `<Ctrl>+ <Alt> + <t>`  
- **Linha de comando "livre"**: Digite `:` e pressione Enter. Para sair, digite `q` e Enter.

## COMANDOS DE NAVEGAÇÃO E ARQUIVOS

- **ls**: Lista arquivos e diretórios da pasta atual.  
- **cd [diretório]**: Acessa o diretório especificado.  
- **cd**: Vai direto para o diretório HOME do usuário.  
- **pwd**: Mostra o caminho completo do diretório atual.  
- **clear**: Limpa a tela do terminal.  
- **cat [arquivo]**: Exibe o conteúdo de um arquivo (equivalente ao `type` no DOS).  
- **df**: Mostra partições usadas ou livres no HD.  
- **| more**: Pagina a saída de um comando linha a linha (ex.: `cat arquivo | more`).  
- **| lpr**: Envia o arquivo para impressão.  
- **vim [arquivo]**: Abre o arquivo no editor Gedit.  
- **konsole**: Abre outro terminal.  

## COMANDOS DE DESLIGAMENTO E REINÍCIO

- **shutdown**: Desliga o computador.  
- **shutdown -r now**: Reinicia imediatamente.  
- **shutdown -h now**: Desliga imediatamente (aguarde mensagem "system halted").  
- **reboot**: Reinicia o sistema instantaneamente (uso recomendado apenas em emergências).  


## COMANDOS DE DIRETÓRIOS E ARQUIVOS

- **mkdir [nome]**: Cria um diretório.  
- **rmdir [nome]**: Remove diretório vazio.  
- **rm [arquivo]**: Remove um arquivo.  
- **rm -r [diretório]**: Remove diretório com conteúdo.  
- **mv [origem] [destino]**: Move ou renomeia arquivos/diretórios.  

## COMANDOS DE USUÁRIOS

- **who**: Mostra quem está usando o sistema.  
- **useradd [nome]**: Cria um novo usuário.  
- **passwd [nome]**: Cria ou altera a senha de um usuário.  
- **userdel -r [nome]**: Remove usuário e seu diretório HOME.  
- **su**: Passa para o superusuário (`$` muda para `#`).  

## COMANDOS DE MEMÓRIA E SISTEMA

- **free**: Mostra a memória do sistema.  
- **date**: Mostra data e hora atual.  
- **ps**: Lista processos em execução.  
- **kill [PID]**: Encerra processo pelo ID.  
- **history**: Mostra os comandos digitados pelo usuário.  

## COMANDOS DE IMPRESSÃO

- **lpr [arquivo]**: Envia arquivo para impressão.  
- **lpq**: Mostra status da fila de impressão.  
- **lprm [ID]**: Remove trabalhos da fila de impressão.  

## COMANDOS DE ARQUIVOS E BACKUPS

- **TAR -c [arquivo]**: Cria backup.  
- **TAR -x [arquivo]**: Restaura backup.  
- **TAR -v [arquivo]**: Lista cada arquivo do backup.  
- **TAR -t [arquivo]**: Lista conteúdo do backup.  

## COMANDOS DIVERSOS

- **type [arquivo]**: Mostra informações sobre um arquivo.  
- **file [arquivo]**: Descreve o tipo de um arquivo.  
- **find / -name** " [arquivo ou nome de arquivos] " -exec ls -lh {} \ : Procura arquivo no diretorio alem de listar.   
- **linuxconf**: Abre ferramenta de configuração do Linux.  
- **alias**: Cria atalhos para comandos.  
- **&**: Executa comando em background.  
- **mtools**: Permite usar ferramentas compatíveis com DOS (comando `M` na frente).  
- **minicom (m)**: Configura modems via terminal.  

---

