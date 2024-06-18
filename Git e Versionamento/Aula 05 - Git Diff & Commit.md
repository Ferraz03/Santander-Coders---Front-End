# Git Diff

O comando `git diff` é usado no Git para exibir as diferenças entre o estado atual do seu diretório de trabalho e o índice (staging area), ou entre o índice e o último commit. Aqui estão algumas formas comuns de usar o `git diff`:

1. **Diferenças entre o diretório de trabalho e o índice**:
    
    ```bash
    git diff
    ```
    
    Este comando mostra as diferenças entre os arquivos no seu diretório de trabalho e o que foi preparado (staged) para o próximo commit.
    
2. **Diferenças entre o índice e o último commit**:
    
    ```bash
    git diff --staged
    ```
    
    Também pode ser escrito como `git diff --cached`. Este comando exibe as diferenças entre os arquivos que estão preparados para o próximo commit (índice) e o último commit confirmado.
    
3. **Diferenças entre dois commits específicos**:
    
    ```bash
    git diff commit1..commit2
    ```
    
    Isso mostra as diferenças entre dois commits específicos. Substitua `commit1` e `commit2` pelos hashes SHA-1 dos commits que você deseja comparar.
    
4. **Diferenças entre um arquivo específico**:
    
    ```bash
    git diff nome-do-arquivo
    ```
    
    Este comando mostra as diferenças específicas de um arquivo em relação ao último commit.
    
5. **Diferenças incluindo renomeamento de arquivos**:
    
    ```bash
    git diff --find-renames
    ```
    
    Isso permite que o Git detecte e mostre mudanças que incluem renomeios de arquivos, em vez de tratá-los como exclusões e adições separadas.
    

O `git diff` é uma ferramenta poderosa para visualizar e entender as mudanças em seu repositório Git antes de fazer um commit. Ele fornece uma visão detalhada das alterações e é útil para revisar o trabalho realizado e garantir que todas as mudanças desejadas sejam incluídas no próximo commit.

<aside>
💡 Aperte a tecla ‘Q’ para sair do `git diff` no terminal

</aside>

# Git Commit

O comando `git commit` é utilizado para confirmar as mudanças feitas nos arquivos que foram preparados (staged) usando `git add` para o repositório. Aqui estão os passos principais envolvidos em realizar um commit com Git:

1. **Preparar os arquivos para commit**:
Antes de realizar um commit, é necessário usar `git add` para adicionar os arquivos desejados ao índice (staging area). Isso prepara as mudanças para serem incluídas no próximo commit.
    
    ```bash
    git add arquivo1.txt arquivo2.txt
    ```
    
    Ou, para adicionar todos os arquivos modificados e novos:
    
    ```bash
    git add .
    ```
    
2. **Confirmar as mudanças**:
Após preparar os arquivos, você pode usar `git commit` para confirmar as mudanças no repositório. Isso abrirá um editor de texto onde você pode inserir uma mensagem descritiva para o commit. A mensagem é importante para descrever de forma clara e concisa o que foi feito nas mudanças.
    
    ```bash
    git commit
    ```
    
    Alternativamente, você pode adicionar a mensagem diretamente na linha de comando:
    
    ```bash
    git commit -m "Mensagem do commit aqui"
    ```
    
3. **Exemplo de commit com mensagem**:
    
    ```bash
    git commit -m "Adiciona novos recursos ao sistema"
    ```
    
    Após confirmar o commit, as alterações são registradas no histórico do repositório Git com a mensagem fornecida. Cada commit cria um ponto na linha do tempo do projeto, facilitando o rastreamento de alterações e a colaboração com outros membros da equipe.
    

Lembre-se de que o `git commit` apenas confirma as mudanças no seu repositório local. Para enviar as alterações para um repositório remoto, você normalmente usaria `git push` após o commit, se estiver trabalhando em um ambiente colaborativo.