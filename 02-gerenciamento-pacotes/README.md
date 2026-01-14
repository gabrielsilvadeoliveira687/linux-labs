
# 02 - GERENCIAMENTO DE PACOTES NO LINUX

## INTRODUÇÃO

# Esta seção explica como funciona o gerenciamento de pacotes em linux, principalmente nas distribuições derivadas do unix. compreender esse processo é fundamental para instalar, atualizar, remover softwares e manter o sistema estável e seguro.

#  cada distribuição pode ter seu próprio gerenciador de pacotes, como `apt`, `yum` ou `dnf`, e é importante sempre saber qual distribuição você está utilizando, por exemplo: `ubuntu`, `debian`, `linux mint`, `arch`, `kali`, `centos` etc.**

---

## gerenciadores de pacotes

### apt (debian, ubuntu e derivados)

**apt (advanced package tool)** é utilizado em distribuições baseadas no debian.**

#### comandos básicos


- **apt update**: atualiza a lista de pacotes disponíveis.  
- **apt upgrade**: atualiza todos os pacotes instalados.  
- **apt install [pacote]**: instala um pacote específico.  
- **apt remove [pacote]**: remove um pacote instalado.  
- **apt search [pacote]**: procura um pacote nos repositórios.


---


### yum e dnf (centos, rhel, fedora)

Em distribuições baseadas no red hat, o gerenciamento de pacotes é feito pelo **yum** ou **dnf**, sendo o dnf a versão mais moderna.

#### Comandos básicos com dnf

- **dnf search [pacote]**: Procura um pacote nos repositórios. 
- **dnf install [pacote]**: Instala um pacote.  
- **dnf remove [pacote]**: Remove um pacote instalado.  
- **dnf update**: Atualiza todos os pacotes do sistema.

---

## verificando a distribuição

Antes de usar qualquer gerenciador de pacotes, é recomendado confirmar a distribuição do sistema:

#bash
- **cat /etc/os-release**

## boas práticas

# Sempre use o gerenciador de pacotes padrão da distribuição para evitar problemas de dependências.
# Mantenha o sistema atualizado para garantir segurança e estabilidade. 
# Ao procurar pacotes, utilize os comandos de busca (apt search ou dnf search) para confirmar o nome exato.

evite instalações manuais fora do gerenciador sem necessidade.

conclusão
