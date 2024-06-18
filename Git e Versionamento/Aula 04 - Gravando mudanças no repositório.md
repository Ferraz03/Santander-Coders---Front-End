# Estados do Git

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/120b5c8b-202a-47d6-b180-84487b666423/e5b34278-1495-496a-987d-df80ccdad7ac/Untitled.png)

1. Untracked  (Não Rastreado)
    1. Arquivos que estão presentes no diretório de trabalho, mas ainda não foram adicionados ao sistema de controle de versão. O Git não gerencia mudanças ou histórico para esses arquivos até que sejam explicitamente adicionados.
2. Unmodified (**Não modificado)**
    1. Arquivos que estão sendo rastreados pelo Git e não foram alterados desde o último commit. O Git reconhece esses arquivos e não os considera para inclusão no próximo commit a menos que sejam modificados.
3. Modifed (Modificado)
    1. Arquivos que foram alterados desde o último commit. Essas mudanças podem estar em progresso e ainda não foram preparadas (staged) para o próximo commit.
4. Staged (Preparado)
    1. Arquivos que foram marcados para serem incluídos no próximo snapshot (instantâneo) do commit. Quando você prepara um arquivo no Git, você está o incluindo para ser commitado, o que significa que o Git vai incluir as mudanças feitas nesse arquivo no próximo snapshot da história do seu projeto.

# Git Status

O comando `git status` é utilizado no Git para verificar o estado atual do seu repositório local. Ele fornece informações sobre quais arquivos estão modificados, quais estão preparados (staged) para commit, e se há alguma diferença entre o repositório local e o repositório remoto (caso exista um repositório remoto configurado).

Quando você executa `git status`, você receberá informações como:

- Quais arquivos foram modificados desde o último commit (`modified`).
- Quais arquivos estão preparados para serem incluídos no próximo commit (`staged`).
- Quais arquivos existem no diretório de trabalho, mas ainda não foram adicionados ao Git (`untracked`).
- Se o seu branch atual está atualizado com o repositório remoto ou se há mudanças que precisam ser puxadas ou enviadas (`ahead` ou `behind`).

# Git Add

O comando `git add` é usado para adicionar alterações de arquivos ao índice (também conhecido como área de preparação ou staging area) do Git, preparando-os para serem incluídos no próximo commit. Aqui estão alguns usos comuns do `git add`:

1. **Adicionar arquivos específicos**:
    
    ```bash
    git add arquivo.txt
    ```
    
    Isso adiciona o arquivo `arquivo.txt` ao índice, marcando-o como preparado para o próximo commit.
    
2. **Adicionar todos os arquivos modificados e novos**:
    
    ```bash
    git add .
    ```
    
    O ponto (`.`) adiciona todos os arquivos modificados e novos (que não são arquivos deletados) no diretório atual e seus subdiretórios ao índice.
    
3. **Adicionar arquivos interativamente**:
    
    ```bash
    git add -i
    ```
    
    Este comando inicia um modo interativo que permite selecionar quais arquivos adicionar ao índice de forma mais detalhada, como adicionar apenas partes específicas de um arquivo (`git add -p`).
    
4. **Adicionar todas as mudanças, incluindo arquivos deletados**:
    
    ```bash
    git add --all
    ```
    
    Este comando adiciona todas as mudanças, incluindo arquivos deletados, ao índice.
    
5. **Adicionar arquivos excluídos**:
    
    ```bash
    git add --all :/
    ```
    
    Este comando adiciona todos os arquivos, incluindo os que foram excluídos, ao índice.
    

É importante lembrar que `git add` não confirma as mudanças no repositório; ele apenas prepara as mudanças para o próximo commit. Após usar `git add` para adicionar os arquivos desejados ao índice, você pode usar `git commit` para confirmar essas mudanças no repositório.

# # Markdown

<aside>
💡 **Arquivo Markdown**

- Um arquivo Markdown é um arquivo de texto simples formatado usando a linguagem Markdown. Markdown é uma linguagem de marcação leve criada por John Gruber e Aaron Swartz que permite que você escreva usando um formato de texto fácil de ler e escrever, que posteriormente pode ser convertido em HTML (ou outros formatos) de forma mais complexa.
- Arquivos Markdown são frequentemente utilizados para escrever conteúdo para a web de uma maneira que seja fácil de ler no seu formato bruto e que possa ser facilmente convertido para HTML para publicação online. Eles são comumente usados em blogs, fóruns, páginas de documentação, e em qualquer lugar onde o texto formatado simples seja necessário.
</aside>