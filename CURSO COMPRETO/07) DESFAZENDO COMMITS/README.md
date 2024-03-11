# DESFAZENDO COMMITS
Desfazer commits no Git envolve o uso de alguns comandos específicos, dependendo de como você deseja desfazer as alterações. Aqui estão algumas maneiras de desfazer commits:

## 1. Desfazer o Último Commit:
Se você cometeu algo acidentalmente e deseja desfazer apenas o último commit, pode usar o seguinte comando:

```shell
git reset HEAD~1
```

Isso irá desfazer o último commit, mas deixará as alterações no seu diretório de trabalho. Você pode então fazer as alterações necessárias e criar um novo commit com as correções.

## 2. Desfazer Commits Anteriores (sem perder alterações):
Se você deseja desfazer commits anteriores, mas manter as alterações em seu diretório de trabalho, pode usar o comando `git reset` com a opção `--soft`. Por exemplo, para desfazer os últimos três commits:

```shell
git reset --soft HEAD~3
```

Isso moverá a branch atual (por exemplo, `master`) para três commits antes do commit atual, mantendo as alterações no seu diretório de trabalho. Você pode então fazer as alterações necessárias e criar um novo commit.

## 3. Descartar Commits Anteriores (perdendo alterações):
Se você deseja desfazer commits anteriores e também descartar as alterações no seu diretório de trabalho, você pode usar o comando `git reset` com a opção `--hard`. Por exemplo, para desfazer os últimos três commits e descartar as alterações:

```shell
git reset --hard HEAD~3
```

Este comando removerá os últimos três commits, bem como as alterações associadas, deixando o seu diretório de trabalho no estado dos commits anteriores.

## 4. Reverter um Commit Específico:
Outra opção é usar o comando `git revert` para criar um novo commit que desfaça as alterações introduzidas por um commit específico. Por exemplo, para reverter o commit com o hash `<hash-do-commit>`:

```shell
git revert <hash-do-commit>
```

O comando `git revert` cria um novo commit que desfaz as alterações introduzidas pelo commit especificado, mantendo o histórico de alterações completo.

## 5) Desfazer o Último Commit com `git checkout`:
### Mantendo Alterações:
Se você deseja desfazer o último commit, mas manter as alterações em seu diretório de trabalho, pode usar o seguinte comando:

```shell
git checkout HEAD~1
```

Isso moverá a branch atual (por exemplo, `master`) para o commit anterior, mas manterá as alterações em seu diretório de trabalho. Você pode então fazer as alterações necessárias e criar um novo commit.

### Descartando Alterações:
Para desfazer o último commit e descartar todas as alterações, você pode usar o comando `git checkout` com a opção `-f` (force):

```shell
git checkout -f HEAD~1
```

Isso descarta todas as alterações no seu diretório de trabalho e move a branch atual para o commit anterior.

Lembre-se de que usar `git checkout` para desfazer commits é útil quando você deseja manter as alterações no seu diretório de trabalho e criar um novo commit posteriormente. Se você quiser remover commits anteriores permanentemente, pode usar o `git reset` com a opção `--hard`, como mencionado anteriormente. Certifique-se de escolher a abordagem que melhor atende às suas necessidades específicas.

**Importante:** Lembre-se de que, se você já compartilhou seus commits com outras pessoas ou enviou-os para um repositório remoto, é melhor evitar usar `git reset --hard` para não causar problemas de consistência no histórico compartilhado. Em vez disso, considere usar `git revert` para criar um novo commit de reversão.

Certifique-se de substituir `<hash-do-commit>` pelo hash do commit que deseja desfazer ou reverter.