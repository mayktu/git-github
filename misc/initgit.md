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

[Conectando arquivos locais com Github](https://github.com/mayktu/git-github/blob/master/misc/conecghub.md)

[Voltar](https://github.com/mayktu/git-github)