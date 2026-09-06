# Template HTML e CSS

Template inicial para projetos de Desenvolvimento Web do Instituto Federal
Catarinense (IFC), desenvolvidos apenas com HTML e CSS.

O repositório oferece uma estrutura simples e configurações compartilhadas de
formatação para que os projetos da turma mantenham o mesmo padrão de
organização.

## Tecnologias e ferramentas

- HTML5;
- CSS3;
- EditorConfig;
- Prettier;
- Visual Studio Code.

## Como utilizar

1. Clique em **Use this template** e selecione **Create a new repository**;
2. defina o nome solicitado para a atividade;
3. clone o novo repositório em seu computador;
4. abra a pasta completa do projeto no Visual Studio Code;
5. instale as extensões recomendadas pelo editor;
6. substitua o conteúdo inicial pelo conteúdo do seu projeto.

> O repositório criado a partir deste template será independente do original.
> Portanto, utilize **Use this template**, e não **Fork** ou **Clone**.

## Estrutura do projeto

```text
seuProjeto
├── .vscode/
│   ├── extensions.json
│   └── settings.json
├── css/
│   └── global.css
├── docs/
│   ├── criar-repositorio-base.md
│   └── guia-padronizacao-codigo.md
├── img/
│   └── .gitkeep
├── .editorconfig
├── .gitignore
├── .prettierignore
├── .prettierrc.json
├── index.html
├── LICENSE
└── README.md
```

O arquivo `.gitkeep` mantém o diretório `img/` no versionamento enquanto ele
estiver vazio. Depois de adicionar a primeira imagem, esse arquivo pode ser
removido.

## Documentação

- [Guia de padronização do código](./docs/guia-padronizacao-codigo.md): explica
  o EditorConfig, o Prettier, as configurações do VS Code e as extensões;
- [Como criar um repositório-base](./docs/criar-repositorio-base.md): apresenta
  o processo de criação e configuração de um template semelhante a este.

## Primeiros ajustes no seu projeto

Depois de criar seu repositório:

- atualize o título e o conteúdo do `index.html`;
- desenvolva os estilos em `css/global.css`;
- armazene as imagens do projeto em `img/`;
- substitua este README pela apresentação e pelas instruções da atividade;
- mantenha os arquivos de configuração versionados.

## Autoria

Desenvolvido pelo [Prof. Cristofer Sousa](https://github.com/cristofersousa)
como material de apoio às atividades de Desenvolvimento Web do Instituto
Federal Catarinense — Campus Araquari.

| Informação  | Descrição                                         |
| ----------- | ------------------------------------------------- |
| Instituição | Instituto Federal Catarinense — Campus Araquari   |
| Curso       | Técnico em Redes de Computadores                  |
| Disciplina  | Desenvolvimento Web I                             |
| Organização | [IFC Dev Web II](https://github.com/ifc-dev-web2) |

## Licença

Este projeto está disponível sob os termos definidos no arquivo
[LICENSE](./LICENSE).
