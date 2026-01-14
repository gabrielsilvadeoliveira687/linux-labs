# 04 - PERMISSÕES E USUÁRIOS NO LINUX

## INTRODUÇÃO

**Esta seção aborda a gestão de usuários, grupos e permissões no Linux**, fundamentais para manter a segurança e organização do sistema. Entender essas permissões é essencial para controlar o acesso a arquivos, diretórios e comandos.

## USUÁRIOS

- **root**: Superusuário do sistema, possui todos os privilégios.  
- **usuário comum**: Possui permissões limitadas, geralmente dentro do seu diretório HOME.  
- **comando who**: Mostra quem está logado no sistema.  
- **comando id [usuário]**: Exibe UID, GID e grupos do usuário.  
- **useradd [nome]**: Cria um novo usuário.  
- **passwd [nome]**: Define ou altera a senha do usuário.  
- **userdel -r [nome]**: Remove usuário e seu diretório HOME.  

## GRUPOS

- **groupadd [nome]**: Cria um novo grupo.  
- **usermod -aG [grupo] [usuário]**: Adiciona usuário a um grupo.  
- **groups [usuário]**: Mostra os grupos que o usuário pertence.  
- **gpasswd -d [usuário] [grupo]**: Remove usuário de um grupo.  

## PERMISSÕES DE ARQUIVOS

No Linux, cada arquivo ou diretório possui **permissões de leitura (r), escrita (w) e execução (x)**, atribuídas a três tipos de usuários:

- **Usuário (owner)**: Dono do arquivo.  
- **Grupo (group)**: Grupo associado ao arquivo.  
- **Outros (others)**: Todos os demais usuários.  

Exemplo de listagem de permissões com `ls -l`:

## INTRODUÇÃO

**Esta seção aborda a gestão de usuários, grupos e permissões no Linux**, fundamentais para manter a segurança e organização do sistema. Entender essas permissões é essencial para controlar o acesso a arquivos, diretórios e comandos.

## USUÁRIOS

- **root**: Superusuário do sistema, possui todos os privilégios.  
- **usuário comum**: Possui permissões limitadas, geralmente dentro do seu diretório HOME.  
- **comando who**: Mostra quem está logado no sistema.  
- **comando id [usuário]**: Exibe UID, GID e grupos do usuário.  
- **useradd [nome]**: Cria um novo usuário.  
- **passwd [nome]**: Define ou altera a senha do usuário.  
- **userdel -r [nome]**: Remove usuário e seu diretório HOME.  

## GRUPOS

- **groupadd [nome]**: Cria um novo grupo.  
- **usermod -aG [grupo] [usuário]**: Adiciona usuário a um grupo.  
- **groups [usuário]**: Mostra os grupos que o usuário pertence.  
- **gpasswd -d [usuário] [grupo]**: Remove usuário de um grupo.  

## PERMISSÕES DE ARQUIVOS

No Linux, cada arquivo ou diretório possui **permissões de leitura (r), escrita (w) e execução (x)**, atribuídas a três tipos de usuários:

- **Usuário (owner)**: Dono do arquivo.  
- **Grupo (group)**: Grupo associado ao arquivo.  
- **Outros (others)**: Todos os demais usuários.  

Exemplo de listagem de permissões com `ls -l`:





