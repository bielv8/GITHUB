# CONCEITOS DE GIT:
Os conceitos-chave do Git são fundamentais para entender como o Git rastreia e gerencia as alterações em seu projeto de desenvolvimento de software. Aqui estão os principais conceitos do Git:

1. **Repositório .git:**

   - Um repositório Git é um diretório que contém todos os arquivos e metadados relacionados ao controle de versão do seu projeto.
   - Dentro do diretório do seu projeto, o Git cria uma pasta oculta chamada `.git`, que contém informações sobre o histórico de alterações, branches, configurações e outros metadados do projeto.

2. **Commit:**

   - Um commit no Git representa uma alteração específica no seu projeto.
   - Cada commit tem um identificador exclusivo (hash) e uma mensagem descritiva que explica o que foi alterado.
   - Os commits são usados para criar um histórico de alterações e marcam pontos específicos na linha do tempo do projeto.

3. **Modified (Modificado):**

   - Os arquivos do seu projeto são considerados "modificados" quando você faz alterações neles após o último commit.
   - As alterações nos arquivos modificados não foram registradas no Git até que você crie um novo commit.

4. **Staging (Área de Preparação):**

   - Antes de criar um commit, você pode escolher quais alterações deseja incluir nele. Isso é feito adicionando os arquivos modificados à "área de preparação" (staging area) do Git.
   - Os arquivos na área de preparação serão incluídos no próximo commit que você criar.

5. **Committed (Cometido):**

   - Quando você cria um commit, as alterações na área de preparação são registradas permanentemente no histórico do projeto.
   - Os commits são a maneira pela qual o Git mantém o controle das versões e históricos das alterações.

6. **Branch (Ramo):**

   - Um branch no Git é uma linha de desenvolvimento separada do projeto.
   - Você pode criar branches para trabalhar em novos recursos, correções de bugs ou experimentos sem afetar a branch principal.
   - As branches permitem o desenvolvimento paralelo e a colaboração em equipe.
   - A branch principal é frequentemente chamada de "master" ou "main", mas você pode nomeá-la de acordo com suas preferências.

Esses conceitos fundamentais do Git são essenciais para entender como o Git funciona e como você pode gerenciar seu projeto de desenvolvimento de software. Ao criar commits, manipular a área de preparação e trabalhar com branches, você pode controlar efetivamente as alterações no seu projeto e colaborar de maneira eficiente com outros desenvolvedores.