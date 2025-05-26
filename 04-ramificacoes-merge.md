// Git Branch, Checkout.

Branches (ou "ramificações") são cópias independentes do código dentro de um repositório, usadas para desenvolver novas funcionalidades, corrigir bugs ou testar mudanças sem afetar o código principal (geralmente chamado de main ou master).

Ao criar uma branch, você trabalha de forma isolada. Quando termina as alterações, pode abrir um pull request para revisar e, se aprovado, mesclar (merge) essa branch com a main.

Para criar uma branch, basta usar o comando $git branch "nome da branch".

Para mudar para essa minha branch criada, basta usar o comando $git checkout "nome da branch".

Para deletar uma branch que você criou, basta usar o comando $git branch -d "nome da branch"

Também temos o comando $git branch , que lista todas as branchs ativas no projeto.
