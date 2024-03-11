# RESOLVENDO CONFLITOS
Resolver conflitos de mesclagem no Git é uma parte importante do processo de fusão de branches. Conflitos ocorrem quando o Git não consegue automaticamente mesclar as alterações de duas branches devido a edições conflitantes na mesma parte de um arquivo. Para resolver conflitos, você deve manualmente escolher como as alterações devem ser combinadas. Aqui estão os passos para resolver conflitos de mesclagem:

## Passo 1: Identificar Arquivos com Conflitos:
Quando você executa `git merge` e há conflitos, o Git informará quais arquivos têm conflitos e mostrará uma mensagem de erro. Você pode usar o comando `git status` para ver a lista de arquivos com conflitos e identificá-los.

## Passo 2: Abrir Arquivos com Conflitos:
Abra cada arquivo com conflitos em um editor de texto. Os arquivos conterão marcações especiais para indicar as seções conflitantes, como:

```plaintext
<<<<<<< HEAD
// Conteúdo da branch atual (HEAD)
=======
// Conteúdo da outra branch (branch sendo mesclada)
>>>>>>> branch-secundaria
```

Essas marcações indicam onde as alterações de ambas as branches colidem.

## Passo 3: Resolver os Conflitos:
Para resolver os conflitos, você deve escolher qual versão das alterações manter ou combinar as duas versões, dependendo das necessidades do seu projeto. Você pode editar o arquivo para remover as marcações e deixar o código como desejar.

Por exemplo, para resolver um conflito em um arquivo `meu-arquivo.txt`, você pode editar o arquivo para que ele fique como você deseja:

```plaintext
Conteúdo da branch atual (HEAD)
Conteúdo da outra branch (branch sendo mesclada)
```

**Passo 4: Adicionar os Arquivos Resolvidos ao Estágio:**
Depois de resolver os conflitos em um arquivo, você deve adicionar o arquivo ao estágio (staging area) usando o comando `git add`. Isso marca o arquivo como resolvido e pronto para ser confirmado.

```shell
git add meu-arquivo.txt
```

## Passo 5: Continuar a Mesclagem:
Após resolver todos os conflitos e adicionar os arquivos resolvidos ao estágio, você pode continuar o processo de mesclagem executando o comando `git commit` para criar um novo commit que registra a mesclagem.

```shell
git commit -m "Resolvido conflito em meu-arquivo.txt"
```

## Passo 6: Concluir a Mesclagem:
Após confirmar a mesclagem com sucesso, você pode continuar trabalhando na branch mesclada ou descartar a branch secundária, se não for mais necessária.

Lembre-se de que resolver conflitos é uma parte normal do trabalho com Git, especialmente em projetos colaborativos. Sempre revise cuidadosamente as alterações e certifique-se de que a mesclagem resultante seja apropriada para o seu projeto.