# IGNORANDO ARQUIVOS E DIRETORIOS
## ARQUIVOS:
Para ignorar arquivos no Git, você pode usar o arquivo `.gitignore`. O `.gitignore` é um arquivo de configuração que lista os padrões de nomes de arquivos e diretórios que você deseja que o Git ignore. Os arquivos listados no `.gitignore` não serão rastreados pelo Git e não serão incluídos nos commits. Isso é útil para evitar que arquivos temporários, arquivos de compilação, arquivos de configuração local e outros tipos de arquivos desnecessários sejam incluídos no controle de versão.

Aqui estão os passos para criar e usar um arquivo `.gitignore`:

### Passo 1: Crie um arquivo `.gitignore`:
Você pode criar o arquivo `.gitignore` manualmente no diretório raiz do seu projeto ou usar um comando para criá-lo. Para criar manualmente, você pode usar um editor de texto ou o comando `touch`. Por exemplo:

```shell
touch .gitignore
```

### Passo 2: Edite o arquivo `.gitignore`:
Abra o arquivo `.gitignore` em um editor de texto e adicione os padrões de arquivos e diretórios que você deseja ignorar. Cada padrão deve estar em uma linha separada. Por exemplo:

```plaintext
# Ignorar arquivos temporários
*.tmp

# Ignorar diretório de compilação
build/

# Ignorar arquivos de configuração local
config.local
```

Neste exemplo, o Git irá ignorar todos os arquivos com extensão `.tmp`, o diretório `build/` e o arquivo `config.local`.

### Passo 3: Salve e Commit o `.gitignore`:
Depois de adicionar os padrões de ignorar ao `.gitignore`, salve o arquivo e faça um commit para registrar o arquivo `.gitignore` no histórico do Git:

```shell
git add .gitignore
git commit -m "Adicionado arquivo .gitignore"
```

A partir desse ponto, o Git começará a ignorar os arquivos e diretórios listados no `.gitignore` ao criar commits e realizar operações relacionadas ao controle de versão.

Lembre-se de que o arquivo `.gitignore` é específico para cada repositório Git, o que significa que você pode criar diferentes arquivos `.gitignore` para diferentes projetos, dependendo das necessidades do projeto. Certifique-se de adicionar ao `.gitignore` apenas os arquivos e diretórios que são específicos para o seu projeto e que não devem ser compartilhados com outros colaboradores.

## DIRETÓRIOS:
Para ignorar um diretório no Git, você pode adicionar o nome do diretório ao arquivo `.gitignore`. O arquivo `.gitignore` é usado para listar os padrões de nomes de arquivos e diretórios que você deseja que o Git ignore. Quando você adiciona um diretório ao `.gitignore`, o Git não rastreará nenhum arquivo ou subdiretório dentro desse diretório. Aqui estão os passos para ignorar um diretório:

### Passo 1: Crie ou Edite o arquivo `.gitignore`:**
Se você já não tem um arquivo `.gitignore` no diretório raiz do seu projeto, crie um usando um editor de texto ou o comando `touch`:

```shell
touch .gitignore
```

### Passo 2: Edite o arquivo `.gitignore`:
Abra o arquivo `.gitignore` em um editor de texto e adicione o nome do diretório que você deseja ignorar. Certifique-se de incluir uma barra no início para indicar que é um diretório. Por exemplo, se você deseja ignorar um diretório chamado `meu-diretorio`, adicione a seguinte linha ao `.gitignore`:

```plaintext
/meu-diretorio/
```

Isso instruirá o Git a ignorar todo o conteúdo do diretório `meu-diretorio` e quaisquer subdiretórios ou arquivos dentro dele.

## Passo 3: Salve e Commit o `.gitignore`:
Após adicionar o diretório ao `.gitignore`, salve o arquivo e faça um commit para registrar o arquivo `.gitignore` no histórico do Git:

```shell
git add .gitignore
git commit -m "Adicionado diretório ao .gitignore"
```

A partir deste ponto, o Git não rastreará mais os arquivos ou diretórios listados no `.gitignore`. Certifique-se de fazer isso no início do projeto para evitar que os arquivos indesejados sejam incluídos no controle de versão.