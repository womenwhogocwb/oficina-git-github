# Primeira aula de git CODELAB 01

## O que vimos na primeira aula?

### Instalação do GIT

https://git-scm.com/downloads

Obs: para o Windows após a instalação utilizem o programa GitBash que foi instalado junto no pacote. No Linux ou MacOS pode utilizar o terminal já existente no sistema operacional.

❗️ Comandos de terminal para se localizar:

-  `ls` - lista arquivos e pastas
-  `cd` - avança para a pasta selecionada (ex: cd Documents)

### Criação conta no GITHUB

https://github.com

Criação de repositório para um novo projeto no GITHUB.

### Configurar o repositório local

Pelo terminal entro em uma pasta onde quero colocar meu repositório local:

```bash
cd Documentos/projetos/
```

Quando estiver na pasta escolhida, clone o repositório (utilizar modo HTTPS):

```bash
git clone https://github.com/womenwhogocwb/oficina-git-github.git
```

O comando de clone irá criar dentro de Documentos/projetos a pasta com o nome do seu repositório. Então você deve entrar nesta pasta para continuar trabalhando com o git:

```bash
cd wwg
```

Se o seu projeto já tiver arquivos os mesmo também serão baixados nesta pasta.

Caso seja a primeira vez que vc está utilizando o git neste computador, será necessário informar seu e-mail e seu nome para identificar as alterações no projeto.

```bash
git config --global user.email "eu@mesma.com"

git config --global user.name "meu nome"
```


Prontas para começar a brincar no projeto. Criar um arquivo qualquer (pode ser txt ou mesmo um arquivo com código em GO)

Veja o que foi feito com o comando:

```bash
git status
```

Adicione o seu aqui para que o git entenda que você quer enviá-lo ao repositório no GitHub

```bash
git add arquivo.txt
```

Commit (registrar) seu arquivo/alteração sempre informando o que foi feito nele:

```bash
git commit -m "mensagem informando o que foi feito"
```

Veja o histórico de commits com o seguinte comando:

```bash
git log
```

Se estiver tudo pronto para ser publicado, o commando push enviará suas modificações para o repositório remoto:

```bash
git push
```

