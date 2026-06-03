# TIC-Lab-PUCRS

Versionamento de códigos com parceria com +praTI.

# Módulo 01 - Controle de Versão (Básico)

# 🚀 Git e GitHub - Resumo das Aulas 1 a 6 modulo

## 📚 Aula 1 - Controle de Versão

### O que é Controle de Versão?

Controle de versão é o processo de gerenciar, rastrear e monitorar alterações em arquivos e projetos ao longo do tempo.

### Benefícios

* Histórico completo de alterações
* Recuperação de versões anteriores
* Trabalho colaborativo
* Organização do desenvolvimento
* Maior segurança do projeto

### Ferramentas de Controle de Versão

* Git
* SVN (Subversion)
* Mercurial
* CVS
* Bazaar
* Perforce
* TFS
* VSTS

### Git x GitHub

| Git                           | GitHub                             |
| ----------------------------- | ---------------------------------- |
| Sistema de controle de versão | Plataforma de hospedagem de código |
| Funciona localmente           | Funciona na nuvem                  |
| Gerencia versões              | Facilita colaboração               |

**Git = Ferramenta**
**GitHub = Plataforma de Hospedagem**

---

## ⚙️ Aula 2 - Instalação e Configuração

### Instalação do Git

Verificar instalação:

```bash
git --version
```

### Configuração Inicial

Configurar nome:

```bash
git config --global user.name "Seu Nome"
```

Configurar email:

```bash
git config --global user.email "seu@email.com"
```

Verificar configurações:

```bash
git config --list
```

### Visual Studio Code

O VS Code é uma IDE/Editor amplamente utilizada para desenvolvimento e integração com Git.

---

## 🗂️ Aula 3 - Funcionamento do Git

### Criando um Repositório

```bash
git init
```

Verificar arquivos ocultos:

```bash
ls -la
```

### Estrutura de Objetos do Git

#### Blob

Armazena arquivos.

#### Tree

Armazena diretórios.

#### Commit

Armazena versões do projeto.

#### Annotated Tag

Ponteiro para um commit específico.

### Áreas de Trabalho

#### Working Directory

Local onde os arquivos são criados e editados.

#### Staging Area

Área de preparação para o próximo commit.

#### Repository

Local onde os commits são armazenados.

### Fluxo do Git

```text
Working Directory
        ↓
     git add
        ↓
   Staging Area
        ↓
   git commit
        ↓
   Repository
```

### Comandos Básicos do Terminal

```bash
mkdir     # Criar diretório
touch     # Criar arquivo
nano      # Editar arquivo
cat       # Exibir conteúdo
ls        # Listar arquivos
cd        # Navegar entre diretórios
rm        # Remover arquivos
clear     # Limpar terminal
```

---

## 🔄 Aula 4 - Operações Básicas do Git

### Ciclo de Vida dos Arquivos

#### Untracked

Arquivo não monitorado.

#### Modified

Arquivo alterado.

#### Staged

Arquivo preparado para commit.

#### Unmodified

Arquivo sem alterações.

### Comandos Essenciais

Verificar status:

```bash
git status
```

Adicionar arquivo:

```bash
git add arquivo.txt
```

Adicionar todos os arquivos:

```bash
git add .
```

Criar commit:

```bash
git commit -m "Mensagem do commit"
```

Visualizar histórico:

```bash
git log
```

Histórico gráfico:

```bash
git log --graph
```

Remover da Staging Area:

```bash
git rm --cached arquivo.txt
```

### Boas Práticas

* Fazer commits frequentes
* Utilizar mensagens claras
* Verificar status regularmente
* Agrupar alterações relacionadas

---

## 🌿 Aula 5 - Branches, HEAD e Merge

### O que é uma Branch?

Uma branch é uma referência (ponteiro) para um commit.

Branch principal:

```text
main
```

### Criar Branch

```bash
git branch feature/login
```

### Trocar de Branch

```bash
git checkout feature/login
```

### Criar e Trocar ao Mesmo Tempo

```bash
git checkout -b feature/login
```

### Listar Branches

```bash
git branch
```

### Remover Branch

```bash
git branch -d nome-da-branch
```

### HEAD

HEAD representa a posição atual do projeto.

```text
HEAD → main
```

### Merge

Une alterações de uma branch em outra.

```bash
git merge feature/login
```

### Tipos de Merge

#### Fast Forward

O Git apenas avança o ponteiro da branch.

#### 3-Way Merge

O Git cria um novo commit de integração.

### Conflitos

Resolver conflitos manualmente e depois:

```bash
git add .
git commit
```

Cancelar merge:

```bash
git merge --abort
```

### Boas Práticas

* Criar branches para novas funcionalidades
* Realizar commits frequentes
* Fazer merges regularmente
* Utilizar nomes descritivos

---

## ☁️ Aula 6 - Repositórios Remotos

### O que é um Repositório Remoto?

É uma cópia do projeto hospedada em um serviço online para compartilhamento e colaboração.

### Clonar Repositório

```bash
git clone URL
```

Exemplo:

```bash
git clone https://github.com/usuario/projeto.git
```

### Adicionar Repositório Remoto

```bash
git remote add origin URL
```

### Verificar Repositórios Remotos

```bash
git remote -v
```

### Enviar Alterações

```bash
git push origin main
```

### Baixar Alterações

```bash
git pull origin main
```

### Buscar Atualizações

```bash
git fetch
```

### Tracking Branch

Configurar branch monitorada:

```bash
git push --set-upstream origin nome-da-branch
```

### Boas Práticas

* Fazer pull regularmente
* Utilizar branches para novas funcionalidades
* Revisar código antes de merge
* Resolver conflitos rapidamente
* Escrever commits descritivos

---

# 📌 Comandos Mais Importantes

```bash
git init
git status
git add .
git commit -m "mensagem"
git log
git branch
git checkout nome-da-branch
git checkout -b nome-da-branch
git merge nome-da-branch
git clone URL
git remote add origin URL
git push
git pull
git fetch
```

---

# 🎯 Conceitos que Mais Caem em Avaliações

| Conceito          | Definição                           |
| ----------------- | ----------------------------------- |
| Working Directory | Local onde os arquivos são editados |
| Staging Area      | Área de preparação                  |
| Repository        | Local dos commits                   |
| Commit            | Registro de alterações              |
| Branch            | Ponteiro para um commit             |
| HEAD              | Indica onde você está trabalhando   |
| Merge             | União de branches                   |
| Git               | Sistema de versionamento            |
| GitHub            | Plataforma de hospedagem            |
| git add           | Adiciona à Staging Area             |
| git commit        | Salva alterações                    |
| git push          | Envia alterações                    |
| git pull          | Baixa alterações                    |

---

## 🏆 Resumo Final

O Git é um sistema de controle de versão distribuído que permite registrar alterações, trabalhar com branches, integrar mudanças através de merges e colaborar utilizando repositórios remotos hospedados em plataformas como GitHub. Seu fluxo principal consiste em editar arquivos no Working Directory, prepará-los na Staging Area com `git add` e registrá-los no repositório através de `git commit`.