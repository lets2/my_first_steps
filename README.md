Questão 1) Meu repositório:
 https://github.com/lets2/my_first_steps

Questão 2)
Acessei o diretório local “my_diretory” usando “cd”
Ao entrar no diretório de interesse, usei o 
git init
Vinculando o diretório local no pc com o repositório remoto
git remote add origin https://github.com/lets2/my_first_steps
Verificando a origem adicionada ao repositório
$ git remote -v
origin  https://github.com/lets2/my_first_steps (fetch)
origin  https://github.com/lets2/my_first_steps (push)

Questão 3)
Depois que criei o arquivo ola_mundo.txt, usei o comando 
$ git status

Usei o comando para adicionar nas mudanças
git add ola_mundo.txt
Depois usei novamente o comando git status para verificar o status
$ git status
On branch master
No commits yet
Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   ola_mundo.txt

git commit -m "Adicionando um arquivo txt"
$  git commit -m "Adicionando um arquivo txt"
[master (root-commit) 3ef6624] Adicionando um arquivo txt
 1 file changed, 4 insertions(+)
 create mode 100644 ola_mundo.txt

$ git push origin master
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 317 bytes | 317.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/lets2/my_first_steps
 * [new branch]      master -> master

Questão 4)
Como não existe o arquivo “.gitignore” uso o comando
cat > ".gitignore"
serei_ignorado.txt
usei ctrl+C para sair

Usei git status pra ver a situação

Depois git add .
$ git add .
warning: in the working copy of '.gitignore', LF will be replaced by CRLF the next time Git touches it

$ git commit -m "Usei o gitignore ignorando um arquivo txt"
[master 878234e] Usei o gitignore ignorando um arquivo txt
 1 file changed, 1 insertion(+)
 create mode 100644 .gitignore
 
Por fim, para atualizar  no diretório remoto então fica:
$ git push --set-upstream origin master
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 320 bytes | 320.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/lets2/my_first_steps
   3ef6624..878234e  master -> master
branch 'master' set up to track 'origin/master'.
