# INSTALAÇÃO E CONFIGURAÇÃO
Este guia oferece instruções passo a passo sobre como instalar o Git, criar uma conta no GitHub e configurar o Git para trabalhar com o GitHub.

## Instalação do Git

O Git é uma ferramenta de controle de versão amplamente usada e está disponível para várias plataformas. Siga os passos abaixo para instalá-lo no seu sistema:

### Passo 1: Baixe o Git
- Para sistemas Windows, acesse o site oficial do Git em [https://git-scm.com/download/win](https://git-scm.com/download/win) e baixe o instalador apropriado para sua versão do Windows.
- Para sistemas macOS, você pode usar o Homebrew. Execute o seguinte comando no Terminal:

  ```shell
  brew install git
  ```

- Para sistemas Linux, use o gerenciador de pacotes da sua distribuição para instalar o Git. Por exemplo, no Ubuntu, você pode usar:

  ```shell
  sudo apt-get install git
  ```

### Passo 2: Instale o Git
- Siga as instruções do instalador para concluir a instalação.

### Passo 3: Verifique a Instalação
- Após a instalação, abra um terminal ou prompt de comando e execute o seguinte comando para verificar se o Git foi instalado com sucesso:

  ```shell
  git --version
  ```

## Criando uma Conta no GitHub
O GitHub é uma plataforma para hospedar projetos Git e colaborar com outros desenvolvedores. Siga os passos abaixo para criar uma conta no GitHub:

### Passo 1: Acesse o GitHub
- Abra seu navegador e acesse [https://github.com/](https://github.com/).

### Passo 2: Crie uma Conta
- Clique no botão "Sign up" (Registrar-se) na página inicial do GitHub.
- Siga as instruções para criar sua conta, incluindo a escolha de um nome de usuário, senha e endereço de e-mail.

### Passo 3: Verifique seu Endereço de E-mail
- Após criar sua conta, o GitHub enviará um e-mail de verificação para o endereço fornecido. Verifique seu e-mail e siga as instruções para confirmar sua conta.

## Configurando o Git com o GitHub
Para configurar o Git para se integrar com o GitHub, siga os passos abaixo:

### Passo 1: Configure seu Nome de Usuário e E-mail
- Abra um terminal ou prompt de comando e execute os seguintes comandos, substituindo `<Seu Nome>` e `<Seu E-mail>` pelos seus próprios dados:

  ```shell
  git config --global user.name "Seu Nome"
  git config --global user.email "seu-email@example.com"
  ```

### Passo 2: Gere uma Chave SSH (Opcional, mas Altamente Recomendado)
- Para uma maior segurança e autenticação com o GitHub, é altamente recomendado gerar uma chave SSH e adicioná-la à sua conta do GitHub. Siga o guia oficial do GitHub em [Generating a new SSH key and adding it to the ssh-agent](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent) para obter instruções detalhadas.

### Passo 3: Adicione sua Chave SSH ao GitHub
- Depois de gerar uma chave SSH, siga o guia oficial do GitHub em [Adding a new SSH key to your GitHub account](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account) para adicionar sua chave SSH à sua conta do GitHub.

Agora você está pronto para usar o Git com sua conta do GitHub!

## Recursos Adicionais
- [Documentação do Git](https://git-scm.com/doc): Consulte a documentação oficial do Git para aprender mais sobre o Git e suas funcionalidades.
- [Guia do GitHub](https://guides.github.com/): O GitHub oferece uma série de guias e recursos úteis para ajudar você a começar e colaborar em projetos.
- [CMDER](https://cmder.app/): Se você usa Windows, pode instalar esse emulador de console.

---

Este guia deve ajudar você a instalar o Git, criar uma conta no GitHub e configurar o Git para se integrar facilmente com o GitHub. Lembre-se de que o GitHub é uma plataforma poderosa para colaboração em projetos de código aberto e desenvolvimento de software em equipe.

# GERENCIANDO VIA CMD:
## DIRETÓRIOS:
Aqui estão alguns comandos do CMD (Prompt de Comando) para gerenciar diretórios (pastas) no Windows:

**1. Criar um Diretório:**
   
   Para criar um novo diretório, você pode usar o comando `mkdir` (make directory) seguido do nome do diretório que deseja criar. Por exemplo:
   
   ```shell
   mkdir NomeDoDiretorio
   ```

**2. Renomear um Diretório:**

   Para renomear um diretório, você pode usar o comando `ren` (rename) seguido do nome atual do diretório e do novo nome. Por exemplo:

   ```shell
   ren NomeDoDiretorio NovoNomeDoDiretorio
   ```

**3. Copiar um Diretório:**

   Para copiar um diretório e seu conteúdo, você pode usar o comando `xcopy` seguido do caminho do diretório de origem e do destino. Por exemplo:

   ```shell
   xcopy C:\Caminho\Origem C:\Caminho\Destino /s /e
   ```

   - `/s` copia diretórios e subdiretórios.
   - `/e` copia diretórios vazios.

**4. Mover um Diretório:**

   Para mover um diretório e seu conteúdo para outro local, você pode usar o comando `move` seguido do caminho do diretório de origem e do destino. Por exemplo:

   ```shell
   move C:\Caminho\Origem C:\Caminho\Destino
   ```

**5. Apagar um Diretório:**

   Para apagar um diretório e seu conteúdo, você pode usar o comando `rmdir` (remove directory) seguido do nome do diretório. Por exemplo:

   ```shell
   rmdir NomeDoDiretorio
   ```

   - Use `/s` para remover diretórios e subdiretórios e `/q` para fazer isso silenciosamente (sem confirmações).

**6. Listar Diretórios e Arquivos:**

   Para listar os diretórios e arquivos em um diretório, você pode usar o comando `dir`. Por exemplo:

   ```shell
   dir
   ```

   Você pode adicionar várias opções ao comando `dir` para personalizar a listagem, como `/b` para listar apenas os nomes dos arquivos e diretórios.

**7. Mudar de Diretório:**

   Como mencionado anteriormente, você pode usar o comando `cd` (change directory) para navegar entre diretórios. Por exemplo:

   ```shell
   cd NomeDoDiretorio
   ```

   Você também pode usar `cd ..` para navegar para o diretório pai.

Lembre-se de que o uso desses comandos pode afetar seu sistema de arquivos, por isso tenha cuidado ao usá-los e verifique duas vezes antes de executar comandos de exclusão ou renomeação, especialmente em diretórios críticos.

## ARQUIVOS:
Vou listar alguns comandos de gerenciamento de arquivos específicos no Windows:

1. **copy**: Copia um ou mais arquivos de um local para outro. Por exemplo, `copy arquivo.txt destino\`.

2. **move**: Move um ou mais arquivos de um local para outro. Isso também pode ser usado para renomear arquivos. Por exemplo, `move arquivo.txt novo_nome.txt`.

3. **ren (rename)**: Renomeia um arquivo. Por exemplo, `ren arquivo_antigo.txt arquivo_novo.txt`.

4. **del (delete)**: Exclui um arquivo. Por exemplo, `del arquivo.txt`.

5. **type**: Exibe o conteúdo de um arquivo de texto diretamente no prompt de comando. Por exemplo, `type arquivo.txt`.

6. **edit**: Abre o editor de texto padrão do Windows para editar um arquivo. Por exemplo, `edit arquivo.txt`.

7. **find**: Procura por uma sequência de texto específica dentro de um arquivo de texto. Por exemplo, `find "palavra" arquivo.txt`.

8. **sort**: Classifica as linhas de um arquivo de texto em ordem alfabética. Por exemplo, `sort arquivo.txt`.

9. **more**: Exibe o conteúdo de um arquivo de texto de forma paginada. Por exemplo, `more arquivo.txt`.

10. **fc (file compare)**: Compara dois arquivos de texto e mostra as diferenças entre eles. Por exemplo, `fc arquivo1.txt arquivo2.txt`.

Lembre-se de que esses comandos são específicos para o gerenciamento de arquivos e não afetam diretórios. Certifique-se de usar esses comandos com cuidado para evitar a perda acidental de dados.