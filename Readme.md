# Lidando com Git e Github

Baby steps on GIT and GITHUB

<p align="center">
<img src="git-github.jpg" width="200" alt="git+github">
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

**para criar um branch**
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
-