# Git Merge

O comando `git merge` é usado para integrar as alterações de uma ramificação (branch) para outra no Git. A operação básica do `git merge` é combinar o histórico de commits de uma ramificação com outra, geralmente fundindo as mudanças feitas em uma ramificação em outra ramificação.

## Como usar `git merge`:

1. **Mudança para a Ramificação Destino**:
Antes de mesclar, você precisa mudar para a ramificação de destino onde deseja incorporar as mudanças. Por exemplo, para mesclar as mudanças da ramificação `feature` na ramificação `main`:
    
    ```bash
    git checkout main
    ```
    
    Ou, se estiver usando Git mais recente:
    
    ```bash
    git switch main
    ```
    
2. **Executar o Merge**:
Após mudar para a ramificação de destino, você pode executar o merge da seguinte forma:
    
    ```bash
    git merge <ramificação-de-origem>
    ```
    
    Por exemplo, para mesclar a ramificação `feature` na ramificação `main`:
    
    ```bash
    git merge feature
    ```
    
    Este comando mescla todos os commits da ramificação `feature` na ramificação `main` e cria um novo commit de merge que une as linhas de desenvolvimento das duas ramificações.
    
3. **Resolução de Conflitos**:
Se houver conflitos entre os commits que estão sendo mesclados, o Git pausará o processo de merge e indicará quais arquivos têm conflitos. Você precisará resolver esses conflitos manualmente, editando os arquivos para incorporar as mudanças corretamente. Depois de resolver os conflitos, você precisa adicionar os arquivos modificados usando `git add` e, em seguida, continuar o merge usando `git merge --continue` ou `git commit` para finalizar o merge.
4. **Finalização do Merge**:
Uma vez resolvidos os conflitos e confirmada a finalização do merge, o Git cria um novo commit de merge na ramificação de destino (`main`, no exemplo acima), incorporando todas as alterações da ramificação de origem (`feature`, no exemplo acima).

## Opções Adicionais:

- `no-ff`: Força o Git a sempre criar um commit de merge, mesmo que seja possível um merge rápido (fast-forward).
- `-abort`: Aborta o processo de merge em caso de problemas.

## Considerações:

- **História de Commits**: O merge preserva o histórico de commits de ambas as ramificações, mostrando quando e onde as mudanças foram integradas.
- **Branches**: É uma prática comum mesclar branches de feature (funcionalidade) de volta à branch principal (como `main` ou `master`) após a conclusão do desenvolvimento e testes.

O `git merge` é uma operação fundamental no Git para integrar e consolidar o trabalho de várias pessoas ou de diferentes funcionalidades em um projeto, garantindo que as alterações sejam combinadas de maneira eficiente e segura.