# CalculaIdade

Comandos Utilizados

Aqui está a explicação resumida de cada comando para integrar diretórios locais com remoto no GitHub.

echo "# DiferencaIdade" >> README.md → Cria um arquivo README.md com o texto # DiferencaIdade (um título em Markdown).

git init → Inicializa um repositório Git na pasta atual (cria a estrutura oculta .git/).

git add README.md → Adiciona o arquivo README.md ao Staging Area (preparação para o commit).

git commit -m "first commit" → Cria um commit com as alterações adicionadas, usando a mensagem "first commit".

git branch -M main → Renomeia a branch padrão (geralmente master) para main (convenção moderna).

git remote add origin https://github.com/User/Diretório(repositório).git → Vincula o repositório local a um repositório remoto (GitHub) chamado origin.

git push -u origin main → Envia (push) os commits locais para o repositório remoto (origin), na branch main. → O -u define origin/main como upstream (rastreamento automático).

Resumo Geral: Esses comandos criam um novo projeto Git, adicionam um README.md, fazem o primeiro commit e o enviam para um repositório remoto no GitHub.


***************************************************************************************************************************

walter-domiciano:~/development/Exercicios/CalculaIdade(git:main)$ git branch 
walter-domiciano:~/development/Exercicios/CalculaIdade(git:main)$ ls
CalculaIdade.iml  out  src
walter-domiciano:~/development/Exercicios/CalculaIdade(git:main)$ git push -u origin main
error: src refspec main does not match any
error: failed to push some refs to 'origin'
walter-domiciano:~/development/Exercicios/CalculaIdade(git:main)$ git add .
walter-domiciano:~/development/Exercicios/CalculaIdade(git:main)$ git push -u origin main
error: src refspec main does not match any
error: failed to push some refs to 'origin'
walter-domiciano:~/development/Exercicios/CalculaIdade(git:main)$ git init
Reinitialized existing Git repository in /home/walter-domiciano/development/Exercicios/CalculaIdade/.git/
walter-domiciano:~/development/Exercicios/CalculaIdade(git:main)$ git add README.md
fatal: pathspec 'README.md' não encontrou nenhum arquivo
walter-domiciano:~/development/Exercicios/CalculaIdade(git:main)$ touch README.md
walter-domiciano:~/development/Exercicios/CalculaIdade(git:main)$ echo "# CalculaIdade" >> README.md
walter-domiciano:~/development/Exercicios/CalculaIdade(git:main)$ git init
Reinitialized existing Git repository in /home/walter-domiciano/development/Exercicios/CalculaIdade/.git/
walter-domiciano:~/development/Exercicios/CalculaIdade(git:main)$ git commit -m "first commit"
[main (root-commit) 3569596] first commit
 9 files changed, 107 insertions(+)
 create mode 100644 .gitignore
 create mode 100644 .idea/.gitignore
 create mode 100644 .idea/aws.xml
 create mode 100644 .idea/material_theme_project_new.xml
 create mode 100644 .idea/misc.xml
 create mode 100644 .idea/modules.xml
 create mode 100644 .idea/vcs.xml
 create mode 100644 CalculaIdade.iml
 create mode 100644 src/Main.java
walter-domiciano:~/development/Exercicios/CalculaIdade(git:main)$ git branch -M main
walter-domiciano:~/development/Exercicios/CalculaIdade(git:main)$ git remote add origin https://github.com/Walterdev1k/CalculaIdade.git
walter-domiciano:~/development/Exercicios/CalculaIdade(git:main)$ git push -u origin main
Enumerating objects: 13, done.
Counting objects: 100% (13/13), done.
Delta compression using up to 4 threads
Compressing objects: 100% (12/12), done.
Writing objects: 100% (13/13), 2.28 KiB | 776.00 KiB/s, done.
Total 13 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/Walterdev1k/CalculaIdade.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.
walter-domiciano:~/development/Exercicios/CalculaIdade(git:main)$ git init && git branch -m main && git add . && git commit -m "Primeiro commit" && git remote add origin https://seu-repositorio.git && git pull origin main --allow-unrelated-histories && git push -u origin main
Reinitialized existing Git repository in /home/walter-domiciano/development/Exercicios/CalculaIdade/.git/
[main 7e74b85] Primeiro commit
 1 file changed, 1 insertion(+)
 create mode 100644 README.md
error: remote origin already exists.
walter-domiciano:~/development/Exercicios/CalculaIdade(git:main)$ git add .
walter-domiciano:~/development/Exercicios/CalculaIdade(git:main)$ git init && git branch -m main && git add . && git commit -m "Primeiro commit" && git remote add origin https://seu-repositorio.git && git pull origin main --allow-unrelated-histories && git push -u origin main
Reinitialized existing Git repository in /home/walter-domiciano/development/Exercicios/CalculaIdade/.git/
No ramo main
Seu ramo está à frente de 'origin/main' por 1 submissão.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean
walter-domiciano:~/development/Exercicios/CalculaIdade(git:main)$ git push -u origin main
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 392 bytes | 392.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/Walterdev1k/CalculaIdade.git
   3569596..7e74b85  main -> main
branch 'main' set up to track 'origin/main'.
