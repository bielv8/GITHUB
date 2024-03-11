# FAZENDO PULL REQUEST (PR)
Um Pull Request (PR) é uma solicitação que você faz a um repositório para que ele puxe (pull) as alterações do seu fork ou branch e as integre ao repositório original. É um recurso fundamental para colaboração em projetos de código aberto e em equipes de desenvolvimento, pois permite que outras pessoas revisem e comentem suas alterações antes de serem mescladas no repositório principal. Aqui estão os passos para criar um Pull Request no GitHub:

## Passo 1: Faça Suas Alterações:
Antes de criar um PR, faça as alterações desejadas no seu fork ou branch local. Certifique-se de confirmar (commit) suas alterações usando `git commit`.

## Passo 2: Crie o Pull Request:
1. Acesse o repositório original no GitHub (não seu fork).
2. Clique na guia "Pull Requests" (PRs) no repositório original.
3. Clique no botão "New Pull Request" (Novo Pull Request).

## Passo 3: Escolha as Branches:
No "Comparing changes" (Comparação de alterações):

- No lado esquerdo, selecione a branch do seu fork ou branch local que contém as alterações que você deseja mesclar.
- No lado direito, selecione a branch de destino, geralmente a branch principal do repositório original.

## Passo 4: Descreva o Pull Request:
Dê um título ao seu PR e escreva uma descrição detalhada que explique o que ele faz. Inclua informações relevantes, contexto e, se necessário, instruções sobre como revisar suas alterações.

## Passo 5: Revisão e Comentários:
Outros colaboradores ou mantenedores do repositório original podem revisar seu PR, fazer comentários e discutir as alterações com você. Isso é feito na guia "Conversations" (Conversas) do PR.

## Passo 6: Resolva os Comentários (se necessário):
Se receber comentários ou solicitações de alterações, você pode fazer as alterações no seu fork ou branch local e confirmá-las (commit) novamente. Os comentários devem ser discutidos e resolvidos até que o PR seja aprovado.

## Passo 7: Mescla do PR:
Depois que o PR for revisado e aprovado, o proprietário do repositório original ou alguém com permissões de gravação poderá mesclá-lo. Isso integrará suas alterações ao repositório original. Você será notificado quando o PR for mesclado.

## Passo 8: Exclusão do Branch (opcional):
Após a mesclagem bem-sucedida do PR, você pode excluir o branch usado para o PR, se não for mais necessário. Isso pode ser feito no GitHub ou usando `git branch -d` localmente.

É importante seguir boas práticas ao criar PRs, como fornecer uma descrição clara e concisa, manter os commits relacionados ao PR organizados e responder prontamente aos comentários dos revisores. Os PRs são uma maneira eficaz de colaborar em projetos Git e garantir que as alterações sejam revisadas e testadas antes da integração.