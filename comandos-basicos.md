# Comandos Básicos do Git

Este guia aborda os comandos essenciais para iniciar seu trabalho com Git. Dominar esses comandos é fundamental para o controle de versão eficiente de seus projetos.

## Índice
1. [git init - Inicializando um repositório](#1-git-init---inicializando-um-repositório)
2. [git status - Verificando o estado](#2-git-status---verificando-o-estado)
3. [git add - Preparando mudanças](#3-git-add---preparando-mudanças)
4. [git commit - Salvando alterações](#4-git-commit---salvando-alterações)
5. [git log - Visualizando histórico](#5-git-log---visualizando-histórico)
6. [Resumo dos Comandos](#resumo-dos-comandos)
7. [Boas Práticas](#boas-práticas)

---

### 1. git init - Inicializando um repositório

Cria um novo repositório Git em um diretório.

```bash
git init
```

O que acontece:

Cria uma subpasta oculta .git com toda a estrutura necessária

Transforma o diretório atual em um repositório versionado

Exemplo:

```bash
mkdir meu-projeto
cd meu-projeto
git init
```
# Saída: Initialized empty Git repository in /caminho/meu-projeto/.git/

### 2. git status - Verificando o estado
Mostra o estado atual do seu repositório.

```bash
git status
```
Informações mostradas:

Branch atual

Mudanças não rastreadas (untracked)

Alterações preparadas para commit (staged)

Arquivos modificados não preparados

# Exemplo de saída:

On branch main
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        arquivo.txt


### 3. git add - Preparando mudanças
Adiciona alterações ao índice (staging area) para o próximo commit.

```bash
# Adicionar arquivo específico
git add arquivo.txt

# Adicionar todos os arquivos modificados
git add .

# Adicionar todos os arquivos .txt
git add *.txt
```
Por que usar:

Permite selecionar quais mudanças serão commitadas

Cria "snapshots" parciais antes do commit final

### 4. git commit - Salvando alterações
Registra as mudanças no repositório com uma mensagem descritiva.

```bash
git commit -m "Mensagem descritiva das alterações"
```
Boas práticas para mensagens:

Comece com verbo no imperativo ("Adiciona", "Corrige", "Remove")

Seja claro e conciso (ideal ≤ 50 caracteres)

Explique o "porquê" no corpo se necessário

Exemplo completo:

```bash
git add index.html style.css
git commit -m "Adiciona estrutura HTML básica e estilos iniciais"
```

### 5. git log - Visualizando histórico
Mostra o histórico de commits do repositório.

```bash
git log
```
Opções úteis:

Comando	Descrição
git log --oneline	Mostra commits resumidos em uma linha
git log -p	Mostra as alterações em cada commit
git log --graph	Exibe o histórico como gráfico de branches
git log --since="2024-01-01"	Filtra por data
Exemplo de saída:

commit 1a2b3c4d5e (HEAD -> main)
Author: Seu Nome <seu@email.com>
Date:   Mon Jan 1 12:00:00 2024 -0300

    Adiciona documentação inicial

## Resumo dos Comandos
Comando	Função	Exemplo
git init	Inicia repositório	git init
git status	Mostra estado atual	git status
git add	Prepara mudanças	git add .
git commit	Grava alterações	git commit -m "msg"
git log	Mostra histórico	git log --oneline