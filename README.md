<p align="center">
  <img alt="vscode logo" src="images/logo-stable.png" width="100px" />
  <h1 align="center">Documentação do Visual Studio Code</h1>
</p>

Você encontrou o repositório GitHub da documentação do Visual Studio Code, que contém o conteúdo para a [Documentação do Visual Studio Code](https://code.visualstudio.com/docs).

Os tópicos enviados aqui serão publicados no portal do [Visual Studio Code](https://code.visualstudio.com).

Se você está procurando pelo repositório GitHub do produto VS Code, você pode encontrá-lo [aqui](https://github.com/Microsoft/vscode).

## Index

1. [Sobre Visual Studio Code](#visual-studio-code)
2. [Feedback](#feedback)
3. [Documentação de Issues](#documentation-issues)
4. [Contribuindo para a documentação](#contributing)
5. [Publicação](#publishing)

## Visual Studio Code

[VS Code](https://code.visualstudio.com/) é um editor de código-fonte leve e um poderoso ambiente de desenvolvimento para criar e depurar aplicativos modernos da Web e da nuvem. É gratuito e está disponível na sua plataforma favorita - Linux, macOS e Windows.

Se você chegou aqui procurando outras informações sobre o VS Code, acesse [nosso site] (https://code.visualstudio.com) para obter informações adicionais.

## Feedback

Se você quiser dar um feedback da documentação, por favor, use o controle de feedback localizado na parte inferior de cada página de documentação.

## Documentação de Issues

To enter documentation bugs, please create a [new GitHub issue](https://github.com/Microsoft/vscode-docs/issues). Please check if there is an existing issue first.

Para inserir erros de documentação, crie um [new GitHub issue] (https://github.com/Microsoft/vscode-docs/issues). Por favor, verifique se existe um problema (issues) existente primeiro.

Se você acha que o problema é com o próprio produto VS Code, insira os problemas no repositório de produtos do VS Code [aqui] (https://github.com/Microsoft/vscode/issues).

## Contribuindo

Para contribuir com novos tópicos / informações ou fazer alterações na documentação existente, leia a [Diretriz Contribuinte] 
(./CONTRIBUTING.md#contributing).

### Workflow

Os dois workflows sugeridos são:

- Para pequenas alterações, use o botão "Edit" em cada página para editar o arquivo Markdown diretamente no GitHub.
- Se você planeja fazer alterações significativas ou visualizar os arquivos Markdown no Código VS, [clone] (#cloning) o repo para [editar e visualizar] (https://code.visualstudio.com/docs/languages/markdown) os arquivos diretamente no código VS.

![Markdown Preview Button](images/MDPreviewButton.png)

### Cloning

1. Instalar [Git LFS](https://git-lfs.github.com/).
2. Rode o comando `git lfs install` para configurar como global o git hooks. Você só precisa executar isso uma vez por máquina.
3. `git clone git@github.com:Microsoft/vscode-docs.git`.
4. Now you can `git add` binary files and commit them. They'll be tracked in LFS.
4. Agora você pode realizar `git add` dos arquivos binários e cometa-los.

#### Cloning without binary files

You might want to clone the repo without the 1.6GB images. Here are the steps:

1. Install [Git LFS](https://git-lfs.github.com/).
2. Run `git lfs install` to setup global git hooks. You only need to run this once per machine.
3. Clone the repo without binary files.
  3.1. macOS / Linux: `GIT_LFS_SKIP_SMUDGE=1 git clone git@github.com:Microsoft/vscode-docs.git`.
  3.2. Windows: `$env:GIT_LFS_SKIP_SMUDGE="1"; git clone git@github.com:Microsoft/vscode-docs.git`.
4. Now you can selectively checkout some binary files to work with. For example:
    - `git lfs pull -I "docs/nodejs"`
    - `git lfs pull -I "release-notes/images/1_3*/*"`
    - You can do `git lfs pull -I <PATTERN>`, as long as `<PATTERN>` is comma-separated glob strings. For more patterns, see [Git LFS: Include and Exclude](https://github.com/git-lfs/git-lfs/blob/master/docs/man/git-lfs-fetch.1.ronn#include-and-exclude).

The history of this repo before we adopted LFS can be found at [microsoft/vscode-docs-archive](https://github.com/Microsoft/vscode-docs-archive).

## Publicação

Passos para a publicação de alterações na documentação podem ser encontrados [aqui](https://github.com/Microsoft/vscode-website#publishing-a-documentation-change) no repositório (privado) do site do VS Code.
