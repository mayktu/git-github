## Contribuindo em outros repositorios

* **Clonando repositorio online para pasta local**
```
git clone HTTPS/SSH DO REPOSITORIO  NOME DA PASTA
```


Quando você clona de outra pessoa você não pode fazer o commit, você tem que fazer o fork para alguma organização, fazer as alterações necessarias e depois fazer um request para a pessoa.



* **Git pull**

Mantem sincronizado as mudanças no repositorio com os arquivos locais, basicamente o inverso do push.
```
git pull
```

* **Manter atualizado um repositorio clonado**
Tenha o fork em seu repositorio
```
git remote add upstream https://github.com/repositorioraiz/repositorioraiz.git
```
```
git remote -v
```
```
git pull upstream master
```

* **Em caso de conflito de arquivos forçar quebra pelo rebase**
```
git pull --rebase upstream master
```
```
git rebase --continue
```
Resolve o conflito e da o push novamente para o repositorio
```
git push --force origin master
```



[Ramificação (Branch)](https://github.com/mayktu/git-github/blob/master/misc/branch.md)

[Voltar](https://github.com/mayktu/git-github)
