# FUNDINDO BRANCHES:
Fusionar (ou mesclar) branches no Git é um processo pelo qual você combina as alterações de uma branch em outra. Isso é geralmente feito quando você concluiu o desenvolvimento de uma funcionalidade ou correção de bug em uma branch secundária e deseja incorporar essas alterações na branch principal. Aqui estão os passos básicos para fundir branches no Git:

## Passo 1: Checkout na Branch de Destino:
Primeiro, certifique-se de estar na branch de destino onde deseja incorporar as alterações da branch secundária. Por exemplo, se você deseja incorporar as alterações da "feature-nova" na branch "main":

```shell
git checkout main
```

## Passo 2: Mesclar a Branch Secundária:
Agora você pode usar o comando `git merge` para mesclar as alterações da branch secundária na branch de destino:

```shell
git merge feature-nova
```

Isso combina as alterações da "feature-nova" na "main". Se houver conflitos entre as alterações (ou seja, se as mesmas partes do código foram modificadas nas duas branches), o Git sinalizará esses conflitos e você precisará resolvê-los manualmente.

## Passo 3: Resolver Conflitos (se necessário):
Se houver conflitos, você precisará resolver esses conflitos manualmente. O Git indicará os arquivos com conflitos e você poderá abrir esses arquivos em um editor de texto para fazer as correções necessárias. Depois de resolver os conflitos, você deve adicionar os arquivos ao estágio (staging area) usando `git add` e, em seguida, continuar o processo de mesclagem com `git commit`.

## Passo 4: Confirmar a Mesclagem:
Após resolver os conflitos (se houver), você pode confirmar a mesclagem com um commit:

```shell
git commit -m "Merge branch 'feature-nova' into main"
```

Isso cria um novo commit que registra a mesclagem da branch secundária na branch de destino. Certifique-se de fornecer uma mensagem significativa para descrever a mesclagem.

## Passo 5: Publicar a Branch de Destino (se necessário):
Se você estiver trabalhando em um repositório Git remoto (como no GitHub), você pode precisar enviar as alterações para o repositório remoto. Você pode fazer isso com `git push`. Por exemplo, para enviar as alterações da "main" para o repositório remoto:

```shell
git push origin main
```

Isso atualiza a branch "main" no repositório remoto com as alterações mescladas.

Depois de seguir esses passos, as alterações da branch secundária estarão incorporadas na branch de destino. Você pode excluir a branch secundária, se desejar, após a mesclagem ser concluída. Lembre-se de que a fusão é uma operação importante, e é importante tomar cuidado ao lidar com conflitos e revisar as alterações antes de confirmar a mesclagem.