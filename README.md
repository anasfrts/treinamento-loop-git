# Aulinha de Git maluka

# Diferença entre Git e Github
![](Versionamento.png)

## O que é Git

## Serviços de hospedagem de repositório
- [Github](https://github.com/)
- [Gitlab](https://about.gitlab.com/)
- [Bitbucket](https://bitbucket.org/product)

---

```
git clone <repositório>
```

```
git checkout -b <nome_da_sua_branch>
```

```
git status
git diff
git add .
git commit -m "Uma mensagem pro seu commit"
```

### Onde tá sua cabeça? (ela sempre tá com você)
(https://git-scm.com/docs/git-checkout#_detached_head/pt_BR)
```
git push origin <nome_da_branch|HEAD>
```

### Hora de fazer o seu MR(Merge Request) / PR(Pull Request)

![](https://i.imgur.com/w4sr7bp.png)

```
git checkout master
git pull origin master|HEAD
git log
```

# Situações que podem acontecer

## Quer criar uma branch a partir de uma remota (tracking)
```
git branch
git fetch origin
git branch
git checkout -b <nome_da_sua_branch_local> origin/<nome_da_branch_remota>
```

## Fez um commit e quer desfazer ele

Quer se desfazer totalmente das mudanças? (Só usar isso quando tiver certeza de que não precisa das mudanças previamente feitas)
```
git reset --hard HEAD~1
```

Quer manter suas mudanças?
```
git reset --soft HEAD~1
```

OU

```
git reset HEAD~1
```

## Quer deletar uma branch
```
git branch -d <nome_da_branch>
git branch -D <nome_da_branch>
```

## Fez mudanças, não quer perder elas e quer algo do remoto
```
git stash
```

E depois:

```
git stash pop
```

## Quer se desfazer de mudanças em um arquivo só
```
git checkout -- <nome_do_arquivo>
```

# Outros conceitos mais diferentões
- Git rebase
- Cherry pick

---
# Mais Conteúdo:
- [História do git](https://www.youtube.com/watch?v=CJtrNuTTs4Q&ab_channel=CursoemV%C3%ADdeo)
- [Docs](https://git-scm.com/docs/git/pt_BR) (tem que adicionar "pt_BR" no fim)
- [Joguim do Abnt](https://learngitbranching.js.org/?locale=pt_BR)
- [Shit shit da Lana](git-cheat-sheet-education.pdf)