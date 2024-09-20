# Estudo Git e GitHub

<br>

## 🖥️ Comandos utilizados no GIT

### Clone de Repositórios:

```
git clone URL-REPOSITORIO
```
### Validando qual sua branch
```
git branch
```
### Criando arquivos dentro do repositório

🚨 **Obs.:** deve ser utilizado no gitBash dentro do diretorio onde fica seu repositório. Com esse comando vc pode criar arquivos dentro do diretorio.
```
touch nome_do_arquivo
```

### Reconhecendo diretórios vazios
    
     Deve ser criado um arquivo com o nome de **.gitkeep** dentro do diretório que se encontra vazio para que o git o reconheça. 


### Adicionando e commitando as alterações realizadas.

```
// Adiciona todas as alterações

git add .


// Adiciona apenas arquivos específicos

git add nome_do_arquivo

// Faz o commit das alterações salvando no repositório local

git commit -m'Mensagem que corresponde a alteração realizada'

// Adicionando tudo e commitando

git add . && git commit -m'Mensagem desejada'

```

### Vizualizando as alterações realizadas e os commits realizados

```
// Visualiza o status da nossa arvore de trabalho 

git status

// Visualiza todos os commits realizados e mostra os hashcodes que são as identificações de cada commit.

git log

// Visualiza todos os commits realizados e mostra os hashcodes que são as identificações de cada commit mais detalhado.

git reflog

```

### Recuperando alterações realizadas

🚨 **Obs.:** Muito cuidado ao utilizar esse comando pois ele descarta todas as alterações realizadas localmente 

```
git restore nome_do_arquivo
```

### Corrigindo commit realizado localmente

🚨 **Obs.:** Muito cuidado ao utilizar esse comando, sempre faça a revisão das alterações antes de usar esses comandos e atenção para o hashcode dos comites. 

```
**Esse comando altera o ultimo commit realizado localmente**

git commit --amend -m'Mensagem que será subistituida'

** Pega os arquivos que estavam nos commits posteriores e os adiciona a área de preparação**

git reset --soft hash_do_commit 

**Pega os arquivos que estavam nos commits posteriores e os adiciona a área de preparação como untracked.**
git reset --mixed hash_do_commit  // pode ser usado git reset


**Remove todas as modificações realizadas**
git reset --hard hash_do_commit 

```


## 📖 Documentação
