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
git push origin :nomedobranch
```

**Merge - Unindo branchs**
##### Pros:
* Operação não destrutiva

##### Contras:
* Historico de commits poluidos
* commit extra (pois ele so uni dois commits)

```
git merge nomedobranch-que-esta-nos-ramos-da-arvore
```

**Rebase - Unindo branchs**

##### Pros: 
* Evita commmits desnecessarios
* Historico linear

##### Contras:

* Perde ordem cronológica

```
git rebase nomedobranch-que-esta-nos-ramos-da-arvore
```


Para saber mais sobre Git branching acesse [Learn Git Branching](https://learngitbranching.js.org/)


[.gitignore](https://github.com/mayktu/git-github/blob/master/misc/gitignor.md)

[Voltar](https://github.com/mayktu/git-github)