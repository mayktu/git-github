# Como trabalhar com Git e Github

Baby steps on GIT and GITHUB

<p align="center">
<img src="./misc/git-github.jpg" width="475" alt="git+github">
</p>

## Configurando o git localmente

**Configurar o nome de usuario**
```
git config --global user.name "NOME DO USUARIO"
git config --global user.email "email do usuario"
```

**Configurando o editor principal (code==visual studio code)**
```
git config --global core.editor code
```

**Consultar nome**
```
git config user.name
```

**Consultar todas as configurações**
```
git config --list 
```



## Inicializando o git e lidando com os arquivos

**Dentro da pasta você para inicializar**
```
git init
```

**Mostrar todos os diretorios**
```
ls -la
```

**Editar o arquivo no editor**
```
code Readme.md
```

**Status atual do seu repositorio**
```
git status
```

**Passando o arquivo para staged**
```
git add nomedoarquivo.ext
```

**Snapshot  depois dos arquivos add**
```
git commit -m "Adicionando Readme.md"
```

**Para adicionar e comitar ao mesmo tempo**
```
git commit -am "Adicionando Readme.md"
```

**Log das versões**
```
git log
git log --graph
```

**Log com mais informações de branch**
```
git log --decorate
```

**Modificaçẽs do autor will**
```
git log --author="Will"
```

**Versão reduzida dos log**
```
git shortlog 
git shortlog -sn
```

**Ver oque aconteceu no commit**
```
git show ff706c2aa70519e5064f94366770f789a7c735
```

**Arquivos modificados e oq foi modificado antes de comitar**
```
git diff
git diff --name-only
```

**Desfazendo a alteração no arquivo**
```
git checkout Readme.md
```

**Resetando as modificações**
```
git reset --short
git reset --mixed
git reset --hard
```



## Conectando arquivos locais com Github
**Codigos para conectar com repositorio online**
```
ssh-keygen -t rsa -b 4096 -C "email@email.com"
ENTER
ENTER
ENTER
```

**SSH para copiar no Github**
```
cd
cd ~/.ssh
ls
cat id_rsa.pub
```

**Passando as coisas do github para o git local**
```
git remote add origin git@github.com:blablablabla
git remote
git remote -v
git push -u origin master
```

## Contribuindo em outros repositorios

**Clonando repositorio online para pasta local**
```
git clone HTTPS/SSH DO REPOSITORIO  NOME DA PASTA
```


Quando você clona de outra pessoa você não pode fazer o commit, você tem que fazer o fork para alguma organização, fazer as alterações necessarias e depois fazer um request para a pessoa.



## Ramificação (Branch)

É um ponteiro movél que leva a um commit

**Para criar um branch**
```
git checkout -b nomedobranch
```

**Para mostrar os branch do repositorio**
```
git branch 
```

**Mudando de branch** 
```
git checkout nomedobranch
```

**Deletando um branch**
```
git branch -D nomedobranch
```

**Merge - Unindo branchs**
Pros:
*Operação não destrutiva

Contras:
*Historico de commits poluidos
*commit extra (pois ele so uni dois commits)

```
git merge nomedobranch-que-esta-nos-ramos-da-arvore
```

**Rebase - Unindo branchs**
Pros: 
*Evita commmits desnecessarios
*Historico linear

Contras:
*Perde ordem cronológica

```
git rebase nomedobranch-que-esta-nos-ramos-da-arvore
```


Para saber mais sobre Git branching acesse [Learn Git Branching](https://learngitbranching.js.org/)


### Gitignore

Ignorar alguns arquivos locais

```
.gitignore
```
Dentro do arquivo .gitignore adiciona os tipos de arquivos que serão ignorados:
```
*json
*py
*c
*cpp
```

[Documentação do gitignore](https://git-scm.com/docs/gitignore)
[Templates para .gitignore](https://github.com/github/gitignore)


### Git Stash
Ele guarda as modificações e aplica em outro branch

```
git stash
```
Entra no outro branch
```
git stash apply
```
Outros comandos:
```
git stash list
git stash clear
```


### Criando atalhos na linha de comando
s substituirá status
```
git config --global alias.s status
```

### Versões com tags

