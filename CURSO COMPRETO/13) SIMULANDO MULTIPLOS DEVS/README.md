# SIMULANDO MULTIPLOS DEVS
## VIA BRANCH:
Para simular o trabalho de múltiplos desenvolvedores em um repositório Git, você pode criar várias branches, cada uma representando o trabalho de um desenvolvedor. Isso é uma prática comum em equipes de desenvolvimento para permitir que os membros trabalhem em diferentes recursos ou correções de bugs de forma isolada e, em seguida, integrem suas alterações ao repositório principal. Aqui está um exemplo de como você pode fazer isso:

Suponha que você tenha um repositório no GitHub chamado `projeto` e deseja simular o trabalho de dois desenvolvedores: DevA e DevB.

## Passo 1: Clone o Repositório:
Clone o repositório do GitHub para o seu computador local usando o comando `git clone`:

```shell
git clone https://github.com/seu-usuario/projeto.git
cd projeto
```

## Passo 2: Crie Branches para os Desenvolvedores:
Crie uma branch para cada desenvolvedor. Vamos criar uma branch chamada `dev-a` para o DevA e uma chamada `dev-b` para o DevB:

```shell
# Crie a branch para o DevA
git checkout -b dev-a

# Faça algumas alterações e commits como DevA
touch arquivo-dev-a.txt
git add arquivo-dev-a.txt
git commit -m "Adicionado arquivo-dev-a.txt"

# Volte para a branch principal (geralmente chamada 'main' ou 'master')
git checkout main

# Crie a branch para o DevB
git checkout -b dev-b

# Faça algumas alterações e commits como DevB
touch arquivo-dev-b.txt
git add arquivo-dev-b.txt
git commit -m "Adicionado arquivo-dev-b.txt"
```

## Passo 3: Integre as Alterações:
Para integrar as alterações dos desenvolvedores de volta à branch principal (ou qualquer outra branch principal que você esteja usando), você pode usar o comando `git merge`. Suponha que você queira integrar as alterações de DevA na branch principal:

```shell
# Volte para a branch principal (main)
git checkout main

# Mescle as alterações de DevA na branch principal
git merge dev-a
```

Repita o processo para integrar as alterações de DevB.

Isso simulará o trabalho de múltiplos desenvolvedores em um projeto Git. Cada desenvolvedor trabalha em sua própria branch, fazendo alterações e commits nela. Quando eles concluem seu trabalho, suas alterações são mescladas de volta à branch principal para manter o código principal atualizado.

Lembre-se de que, em um ambiente de equipe real, você usaria o GitHub ou outra plataforma de hospedagem Git para facilitar a colaboração e garantir que os commits sejam revisados e mesclados de maneira adequada. Além disso, é importante resolver conflitos, se houver, ao mesclar as alterações de diferentes desenvolvedores.

## USANDO O FORK:
Você pode simular o trabalho de múltiplos desenvolvedores em um projeto usando forks em vez de branches. Os forks são cópias independentes de um repositório original, o que é útil quando vários desenvolvedores desejam trabalhar em suas próprias versões do projeto. Aqui está como você pode fazer isso:

## Passo 1: Crie um Fork do Repositório Original:
1. Acesse o repositório original no GitHub que você deseja bifurcar.
2. Clique no botão "Fork" no canto superior direito da página. Isso criará uma cópia do repositório original na sua conta do GitHub.

## Passo 2: Clone o Fork para o seu Computador:
Clone o fork do repositório para o seu computador usando o comando `git clone`:

```shell
git clone https://github.com/seu-usuario/fork-do-projeto.git
cd fork-do-projeto
```

## Passo 3: Trabalhe no seu Fork:
Cada desenvolvedor pode agora trabalhar em seu próprio fork do projeto. Suponha que você seja o DevA:

```shell
# Faça algumas alterações e commits no seu fork como DevA
touch arquivo-dev-a.txt
git add arquivo-dev-a.txt
git commit -m "Adicionado arquivo-dev-a.txt"
```

E o DevB pode fazer o mesmo no seu próprio fork:

```shell
# Faça algumas alterações e commits no seu fork como DevB
touch arquivo-dev-b.txt
git add arquivo-dev-b.txt
git commit -m "Adicionado arquivo-dev-b.txt"
```

## Passo 4: Enviando Pull Requests (PRs):
Quando um desenvolvedor conclui seu trabalho em seu fork e deseja integrar suas alterações ao repositório original (ou ao fork de outro desenvolvedor), ele pode criar um Pull Request (PR). Isso permite que o proprietário do repositório original ou outro desenvolvedor revise as alterações antes de mesclá-las. O processo é o seguinte:

1. No GitHub, vá para o seu fork e clique na guia "Pull Requests".
2. Clique no botão "New Pull Request" (Novo Pull Request).
3. Selecione a branch do seu fork que contém as alterações (por exemplo, `main` ou `dev-a`).
4. Escolha a branch de destino, que pode ser a branch principal do repositório original (por exemplo, `main`).
5. Descreva suas alterações e clique em "Create Pull Request" (Criar Pull Request).

O proprietário do repositório original (ou outro desenvolvedor) pode revisar o PR, discutir as alterações e, se estiverem satisfeitos, mesclar as alterações no repositório original.

**Observação:** Certifique-se de que os desenvolvedores estejam trabalhando em seus próprios forks para evitar conflitos e manter a independência. O processo de forks e PRs é comum em projetos de código aberto e em equipes de desenvolvimento que desejam contribuir para projetos públicos ou colaborar em código privado de forma controlada.