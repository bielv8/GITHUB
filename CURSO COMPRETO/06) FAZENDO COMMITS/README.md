# FAZENDO COMMITS
Para fazer commits no Git, você utiliza o comando `git commit`. Antes de criar um commit, você geralmente adiciona as alterações desejadas à área de preparação (staging area) usando o comando `git add`. Aqui estão os passos para fazer um commit:

## Passo 1: Adicionar Alterações ao Estágio (Staging Area)
Antes de fazer um commit, você precisa adicionar as alterações que deseja incluir no próximo commit à área de preparação. Use o comando `git add` para fazer isso.

```shell
git add arquivo1 arquivo2  # Adicionar arquivos específicos
```

ou

```shell
git add .  # Adicionar todas as alterações
```

## Passo 2: Criar um Commit
Depois de adicionar as alterações à área de preparação, você está pronto para criar um commit. Use o comando `git commit` seguido de uma mensagem que descreva as alterações feitas no commit.

```shell
git commit -m "Mensagem descritiva do commit"
```

Substitua `"Mensagem descritiva do commit"` pela sua própria mensagem, que deve ser concisa e significativa para descrever as alterações feitas.

## Exemplo Completo:
Suponha que você fez alterações em vários arquivos e deseja criar um commit com essas alterações. Aqui está um exemplo completo:

```shell
# Adicionar as alterações à área de preparação (staging)
git add arquivo1 arquivo2

# Criar um commit com uma mensagem descritiva
git commit -m "Adicionei novos recursos e corrigi erros"

# O commit foi criado com sucesso
```

Após executar o comando `git commit`, as alterações são registradas permanentemente no histórico do projeto e o commit é atribuído a você com base nas configurações do Git.

Lembre-se de que os commits são uma parte fundamental do controle de versão do Git e servem para rastrear o histórico de alterações do seu projeto. Portanto, é importante criar commits significativos com mensagens descritivas para facilitar o entendimento das alterações realizadas em cada commit.

# VENDO O HISTÓRICO DE COMMITS:
Para visualizar todo o histórico de commits em um repositório Git, você pode usar o comando `git log`. Este comando exibirá uma lista de commits em ordem cronológica reversa, do mais recente para o mais antigo, juntamente com informações sobre cada commit, como o autor, a data, o identificador único (hash) do commit e a mensagem do commit.

Aqui está como usar o `git log`:

```shell
git log
```

Isso exibirá o histórico de commits no seu repositório. Você pode rolar para baixo para ver mais commits e pressionar a tecla "Q" para sair do visualizador de logs quando terminar de visualizar o histórico.

O comando `git log` possui várias opções e parâmetros para personalizar a saída. Aqui estão alguns exemplos:

## 1. **Limitar o Número de Commits Exibidos:
Você pode limitar o número de commits exibidos usando o parâmetro `-n`, seguido do número desejado. Por exemplo, para mostrar apenas os últimos 5 commits:

   ```shell
   git log -n 5
   ```

## 2. Exibir Alterações em um Arquivo Específico:
Se você deseja ver o histórico de commits para um arquivo específico, você pode passar o caminho do arquivo como um argumento:

   ```shell
   git log caminho/do/arquivo
   ```

## 3. Formatar a Saída:
Você pode personalizar o formato da saída do `git log` usando o parâmetro `--pretty`. Por exemplo, para exibir os commits em um formato mais compacto:

   ```shell
   git log --pretty=oneline
   ```

## 4. Exibir um Gráfico das Ramificações:
Para visualizar um gráfico das ramificações no histórico de commits, use o seguinte comando:

   ```shell
   git log --graph
   ```

## 5. Filtrar por Autor:
Para ver commits de um autor específico, você pode usar o parâmetro `--author`:

   ```shell
   git log --author="Nome do Autor"
   ```

Essas são apenas algumas das opções disponíveis no `git log`. O comando é muito flexível e pode ser ajustado de acordo com suas necessidades específicas para visualizar o histórico de commits de maneira eficiente.