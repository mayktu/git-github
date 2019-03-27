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