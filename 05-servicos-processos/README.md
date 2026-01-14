# 05 - SERVIÇOS E PROCESSOS NO LINUX

## INTRODUÇÃO

**Esta seção aborda o funcionamento de processos e serviços no Linux**, explicando como identificá-los, monitorá-los e controlá-los. Esses conceitos são fundamentais para administração de sistemas, troubleshooting e análise de desempenho.

## PROCESSOS

Um **processo** é uma instância de um programa em execução no sistema. Cada processo possui um identificador único chamado **PID (Process ID)**.

- **ps**: Lista os processos em execução no terminal atual.  
- **ps aux**: Lista todos os processos do sistema.  
- **top**: Exibe os processos em tempo real, com uso de CPU e memória.  
- **htop**: Versão interativa do `top` (necessita instalação).  
- **pgrep [nome]**: Retorna o PID de um processo pelo nome.

## GERENCIAMENTO DE PROCESSOS

- **kill [PID]**: Encerra um processo pelo PID.
- **kill -9 [PID]**: Força o encerramento do processo (uso com cautela).
- **pkill [nome]**: Encerra processos pelo nome.
- **&**: Executa um comando em background.
- **jobs**: Lista processos em background.
- **fg [%job]**: Traz processo em background para foreground.
- **bg [%job]**: Continua um processo em background.

## SERVIÇOS

## Serviços são processos que normalmente rodam em segundo plano (daemons) e iniciam junto com o sistema ou sob demanda.

#Antes de identificar o serviço desejado, utilize sempre o comando ps para verificar quais processos estão em execução no sistema.
#Também é possível utilizar o comando history | grep "nome_do_serviço" para localizar, no histórico do seu usuário, se já houve alguma execução ou referência a esse serviço na máquina.


 SYSTEMD (SISTEMAS MODERNOS)
- **systemctl status [serviço]**: Verifica o status do serviço.
- **systemctl start [serviço]**: Inicia o serviço.
- **systemctl stop [serviço]**: Para o serviço.
- **systemctl restart [serviço]**: Reinicia o serviço.
- **systemctl enable [serviço]**: Habilita o serviço na inicialização.
- **systemctl disable [serviço]**: Remove o serviço da inicialização.

SERVIÇOS EM SISTEMAS LEGADOS (INIT.D)

Em sistemas mais antigos:

- **service [serviço] status**
- **service [serviço] start**
- **service [serviço] stop**
- **service [serviço] restart**

LOGS DE SISTEMA

Logs são fundamentais para identificar erros e comportamentos inesperados.

- **journalctl**: Visualiza logs do systemd.
- **journalctl -u [serviço]**: Logs de um serviço específico.
- **/var/log/**: Diretório padrão de logs do sistema.
- **tail -f [arquivo.log]**: Acompanha logs em tempo real, caso queira um log mais extenso utilze 100f 1000f .

Exemplo:

- **tail -f /var/log/syslog**

### BOAS PRÁTICAS

# Sempre identifique o processo antes de finalizá-lo.
Evite o uso excessivo do kill -9.
Utilize logs para troubleshooting antes de reiniciar serviços.
Monitore consumo de CPU e memória regularmente.

Exemplo:
bash
- **ps aux | grep nginx**
