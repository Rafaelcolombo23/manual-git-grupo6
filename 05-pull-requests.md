GitHub e Pull Requests

1. Criar uma conta no GitHub
-----------------------------
Antes de tudo, você precisa de uma identidade no universo GitHub. 
Acesse https://github.com e crie sua conta com e-mail, nome de usuário e senha.
Depois, capriche no perfil. O GitHub é o seu LinkedIn dos códigos.

2. Criar um repositório remoto
------------------------------
O repositório remoto é o seu cofre na nuvem. Para criar um:

- Clique em "New repository"
- Dê um nome (ex: meu-projeto-zika)
- Escolha se será público ou privado
- (Opcional) Adicione um README.md ou .gitignore
- Clique em "Create repository"

Agora o repositório está disponível para você (e para o mundo, se público).

3. Clonar, Push e Pull
----------------------

CLONAR: Baixa o repositório do GitHub pro seu computador

Comando:
git clone https://github.com/seu-usuario/nome-do-repositorio.git

Isso cria uma cópia local do projeto para você trabalhar.

PUSH: Envia suas alterações locais para o GitHub

Passos:
git add .
git commit -m "feat: minha primeira contribuição épica"
git push origin main

(main pode ser master, depende do nome da branch)

PULL: Puxa atualizações do GitHub para sua máquina

Comando:
git pull origin main

Isso garante que seu código local esteja atualizado com o que está no repositório remoto.

4. Pull Requests e Revisão de Código
------------------------------------

O Pull Request (PR) é uma forma de propor mudanças no projeto. É tipo levantar a mão e dizer: 
"Oi, fiz um código aqui, bora revisar?"

COMO FAZER UM PR:

- Se o projeto não for seu, primeiro faça um fork (cópia do projeto no seu perfil)
- Crie uma nova branch:
  git checkout -b minha-nova-feature
- Faça as alterações e suba normalmente com add, commit, push
- Vá até o GitHub e clique em "Compare & Pull Request"
- Escreva uma descrição do que você fez e envie o PR

REVISÃO:

A equipe (ou o próprio dono do projeto) pode:

- Comentar partes do código
- Sugerir melhorias
- Aprovar ou pedir mudanças

Só depois de tudo aprovado o código é mesclado (merge) com o principal.

Resumo Visual do Ciclo:
[Edita código] -> [git add] -> [git commit] -> [git push] -> [Pull Request] -> [Revisão] -> [Merge]
