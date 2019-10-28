# Segunda parte
###### Ministrada durante o CODELAB 2019

## Hacktoberfest

### O que é o evento?

É uma celebração mundial da comunidade Open Source que ocorre durante o mês de outubro para incentivar a contribuição em projetos de código aberto. 
[Veja mais no site oficial](https://hacktoberfest.digitalocean.com)

Nesta oficina vamos fazer um passo-a-passo para criar seus Pull Requests e poder participar desta celebração. 

Usaremos como exemplo o repositório de exercícios do Codelab, onde cada pessoa irá fazer um fork do projeto e irá adicionar as suas resoluções de exercícios em um repositório próprio através de Pull Request.

### Fork do repositório de exercícios do CODELAB

[https://github.com/womenwhogocwb/WWG-Codelab-01](https://github.com/womenwhogocwb/WWG-Codelab-01)

### Clone o seu fork na máquina local

```bash
$ git clone https://github.com/YOUR_USERNAME/WWG-Codelab-01.git
```

### Crie uma branch para as modificações

```bash
$ git checkout -b nome-da-branch
```

### Adicione e commit suas alterações

```bash
$ git add arquivo_modificado.go

$ git commit -m "descrição da alteração"
```

### Push (empurre) suas alterações para o servidor remoto

```bash
$ git push origin nome-da-branch
```

O retorno deste commando apresenta um link para a branch criada remotamente:
https://github.com/YOUR_USERNAME/WWG-Codelab-01/tree/nome-da-branch

Acesse este link para criar um PULL REQUEST (o famoso PR)

Tome cuidado para escolher para onde será enviado o PULL REQUEST, no nosso caso você deve criar o PR para sua própria conta.    
Clique em 'base repository' para selecionar o seu repositório.

### Manter o repositório atualizado

Caso ocorra alterações no repositório mãe é importante que você sincronize o seu fork.

#### Volte na brach master

```bash
$ git checkout master
> Mudou para a branch 'master'

$ git pull origin master
> Atualizou a branch local
```

#### Configure o upstream

Verifique as configurações remotas
```bash
$ git remote -v
> origin    https://github.com/YOUR_USERNAME/WWG-Codelab-01.git (fetch)
> origin    https://github.com/YOUR_USERNAME/WWG-Codelab-01.git (push)
```

Adicione o repositório mãe como upstream, caso já não esteja configurado
```bash
$ git remote add upstream https://github.com/womenwhogocwb/WWG-Codelab-01.git
```

Verifique novamente as configurações e veja o upstream configurado
```bash
$ git remote -v
> origin    https://github.com/YOUR_USERNAME/WWG-Codelab-01.git (fetch)
> origin    https://github.com/YOUR_USERNAME/WWG-Codelab-01.git (push)
> upstream  https://github.com/womenwhogocwb/WWG-Codelab-01.git (fetch)
> upstream  https://github.com/womenwhogocwb/WWG-Codelab-01.git (push)
```

Sincronize a master do repositório mãe com a sua master
```bash
$ git fetch upstream
$ git merge upstream/master
```
