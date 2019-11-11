#GitHub

git init
cd .git/

1) git-config:


git config --list = tudo que tenho no meu git
git config --global core.editor code = editar editor do git
git config --global user.email = editar email do git 
git config --global user.name = editar nome do git

2) git add:

git add Readme.md = adicionar Readme.md no git


3) git status:

git status = informações do git atual

4) quando salvar algo aqui:

Changes not staged for commit:
arquivo qeu ainda não foi salvo

precisa fazer um git add 

Se quiser salvar mudanças = git commit -m "Add Reame.md"

5) git log:

git log = utilizar bastante para ver as informações

git log = informações dos arquivos
git log -- decorate = informações dos branchs
git log --author="Lincoln" = busca de determinado autor

git shortlog = informações sobre cada contribuinte
git shortlog -sm = pessoa + quant de commit
git log --graph = informações das mudanças em cada branch

git show  = ir no git log, buscar o numero do commit e ver as alterações feitas

6) git diff

git diff= mostrar as diferenças feitas no git para perceber as diferenças feitas na última versão

git diff --name-only = dizer o nome do arquivo que foi modificado 

7) desfazendo coisas

git checkout Readme.md = voltar o arquivo para antes da edição caso faça merda

git add e logo depois
git reset HEAD Readme.md = tirar arquivo do pronto para ser checado


TOMAR CUIDADO:

git reset --soft = qual commit eu quero retornar(ele volta para staged)

git reset --mixed = qual commit eu quero retornar (ele volta para diff)

git reset --hard = mata as informações do último commit

8)Como fazer modificação e mandar direto para o git hub

git remote add origin git@github.com:lincolnanc/gitHubInformations.git
git push -u origin master

Informações desse push
    git remote
    git remote -v

9) Como clonar alguma coisa do git hub para uma pasta local

na home:git clone arquivo clonado nome da pasta
