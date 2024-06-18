# Git Log

O comando `git log` é usado para exibir o histórico de commits de um repositório Git. Ele lista os commits em ordem cronológica reversa (do mais recente para o mais antigo) por padrão. Aqui estão algumas formas comuns de usar o `git log`:

1. **Exibir o histórico de commits**:
    
    ```bash
    git log
    ```
    
    Este comando lista todos os commits no repositório, mostrando informações como o hash SHA-1 do commit, autor, data e mensagem de commit.
    
2. **Limitar o número de commits exibidos**:
    
    ```bash
    git log -n 5
    ```
    
    Isso limita a exibição aos últimos 5 commits. Você pode ajustar o número para exibir mais ou menos commits.
    
3. **Exibir informações resumidas de commits**:
    
    ```bash
    git log --oneline
    ```
    
    Este comando exibe uma lista compacta de commits, mostrando apenas o hash SHA-1 e a mensagem de commit em uma única linha.
    
4. **Exibir diferenças introduzidas em cada commit**:
    
    ```bash
    git log -p
    ```
    
    Adicionando a opção `-p` (ou `--patch`), o `git log` mostra as diferenças introduzidas por cada commit, semelhante ao resultado do `git show` para cada commit.
    
5. **Exibir o histórico de um arquivo específico**:
    
    ```bash
    git log nome-do-arquivo
    ```
    
    Isso mostra o histórico de commits que modificaram um arquivo específico, listando as alterações feitas em cada commit.
    
6. **Exibir o histórico de um determinado autor**:
    
    ```bash
    git log --author="Nome do Autor"
    ```
    
    Este comando lista os commits feitos por um autor específico.
    

O `git log` é uma ferramenta poderosa para explorar o histórico de um projeto Git, permitindo revisar alterações, entender quem fez cada alteração e quando, além de ajudar na investigação de problemas e na colaboração em equipe.

# Git Restore

O comando `git restore` é utilizado no Git para descartar mudanças em arquivos específicos ou para restaurar arquivos ao estado em que estavam em um commit anterior. A funcionalidade exata e o comportamento do `git restore` podem variar dependendo da versão do Git que você está utilizando e das opções específicas que você passa para o comando. Vou cobrir as principais funcionalidades:

## Descartar mudanças em arquivos específicos

Para descartar as mudanças feitas em arquivos específicos e restaurá-los ao estado no último commit, você pode usar:

```bash
git restore nome-do-arquivo
```

Isso restaura o arquivo `nome-do-arquivo` ao estado que estava no último commit, descartando as alterações feitas desde então. Se você já adicionou as mudanças com `git add`, elas serão removidas da área de preparação (staging area).

## Restaurar arquivos ou diretórios ao estado em um commit específico

Para restaurar arquivos ou diretórios inteiros ao estado em um commit específico, você pode usar:

```bash
git restore --source=HEAD~2 --staged --worktree nome-do-arquivo
```

Neste exemplo:

- `-source=HEAD~2` especifica que você deseja restaurar do commit dois commits antes do HEAD (você pode usar qualquer referência de commit válida).
- `-staged` restaura o arquivo na área de preparação (staging area), descartando alterações preparadas.
- `-worktree` restaura o arquivo no diretório de trabalho, descartando alterações que não foram preparadas.

## Opções adicionais

Além disso, você pode usar outras opções com `git restore`, como:

- `-source=<commit>`: Restaura o conteúdo especificado pelo commit.
- `-staged`: Restaura os arquivos na área de preparação.
- `-worktree`: Restaura os arquivos no diretório de trabalho.
- `s` ou `-source`: Usado para especificar a origem (commit) a partir da qual restaurar.

## Versões do Git

É importante notar que o comportamento e as opções do `git restore` podem variar de acordo com a versão do Git que você está usando. Verifique a documentação do Git ou utilize `git restore --help` para obter informações específicas e detalhadas sobre como utilizar o comando na sua versão do Git.