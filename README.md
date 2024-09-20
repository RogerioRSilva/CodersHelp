# Estudo Git e GitHub

<br>

## 🖥️ Codigos utilizados no GIT

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

```

### 

## 📖 Documentação
