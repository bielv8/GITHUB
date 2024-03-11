# COLOCANDO ARQUIVOS NO STAGE:
Para colocar arquivos no estágio (staging area) no Git, você pode usar o comando `git add`. O estágio é onde você prepara as alterações que deseja incluir no próximo commit. Aqui estão alguns exemplos de como usar o comando `git add`:

## Adicionar um Arquivo Específico ao Estágio:

```shell
git add nome-do-arquivo
```

Substitua `nome-do-arquivo` pelo nome do arquivo que você deseja adicionar ao estágio. Isso preparará o arquivo para ser incluído no próximo commit.

## Adicionar Todos os Arquivos Modificados ao Estágio:

```shell
git add .
```

O comando `git add .` adicionará todos os arquivos modificados (novos, modificados e excluídos) no diretório atual e em seus subdiretórios ao estágio.

## Adicionar Arquivos Interativamente ao Estágio:

```shell
git add -i
```

O comando `git add -i` inicia o modo interativo, permitindo que você escolha quais arquivos deseja adicionar ao estágio. Isso é útil quando você deseja uma visão detalhada das alterações antes de adicioná-las.

## Verificar o Status dos Arquivos no Estágio:

Para verificar o status dos arquivos no estágio e os que não estão no estágio, você pode usar o comando `git status`:

```shell
git status
```

Isso mostrará uma lista de arquivos modificados, arquivos no estágio (prontos para commit) e arquivos não rastreados.

Lembre-se de que adicionar arquivos ao estágio é uma etapa importante antes de criar um commit. Uma vez que os arquivos estejam no estágio, você pode usar o comando `git commit` para criar um commit que inclua essas alterações.