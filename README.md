# Nome do projeto

<!--
Substitua “Nome do projeto” pelo nome da atividade e escreva abaixo uma breve
descrição sobre o que foi desenvolvido.
-->

Apresente aqui uma breve descrição do projeto, seus objetivos e o contexto em
que ele foi desenvolvido.

## Tecnologias e ferramentas

- HTML5;
- CSS3;
- EditorConfig;
- Prettier;
- Visual Studio Code.

## Estrutura do projeto

```text
nome-do-projeto/
├── .github/
│   └── pull_request_template.md
├── .vscode/
│   ├── extensions.json
│   └── settings.json
├── css/
│   ├── global.css
│   └── reset.css
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

## Executar o projeto

Abra o arquivo `index.html` utilizando a extensão Live Server do Visual Studio
Code.

Também é possível abrir o arquivo `index.html` diretamente no navegador.

## Documentação

- [Guia de padronização do código](./docs/guia-padronizacao-codigo.md): explica
  o EditorConfig, o Prettier, as configurações do VS Code e as extensões;
- [Como criar um repositório-base](./docs/criar-repositorio-base.md): apresenta
  o processo de criação e configuração de um template semelhante a este.

---

## Orientações para utilizar este template

Este repositório fornece uma estrutura inicial para atividades de
Desenvolvimento Web com HTML e CSS.

### 1. Criar seu repositório

1. Clique em **Use this template**;
2. selecione **Create a new repository**;
3. informe o nome solicitado para a atividade;
4. escolha a visibilidade indicada pelo professor;
5. clique em **Create repository**.

> Não faça um fork nem clone diretamente o repositório-base. Primeiro utilize
> **Use this template** para criar um novo repositório em sua conta.

### 2. Clonar o repositório criado

Acesse o novo repositório em sua conta do GitHub. Clique no botão **Code**,
selecione **HTTPS** e copie o endereço apresentado.

No terminal, acesse o diretório em que deseja armazenar o projeto e execute:

```bash
git clone https://github.com/SEU-USUARIO/NOME-DO-REPOSITORIO.git
```

Entre no diretório criado:

```bash
cd NOME-DO-REPOSITORIO
```

Abra o projeto completo no Visual Studio Code:

```bash
code .
```

> Substitua `SEU-USUARIO` pelo seu usuário do GitHub e
> `NOME-DO-REPOSITORIO` pelo nome definido para a atividade.

### 3. Personalizar o projeto

Depois de criar e clonar o repositório:

- altere o nome e a descrição no início deste README;
- atualize o título e o conteúdo do `index.html`;
- desenvolva os estilos nos arquivos do diretório `css/`;
- armazene as imagens no diretório `img/`;
- mantenha os arquivos de configuração versionados;
- remova estas orientações iniciais quando elas não forem mais necessárias.

## Contexto acadêmico

| Informação | Descrição |
| --- | --- |
| Instituição | Instituto Federal Catarinense — Campus Araquari |
| Curso | Técnico em Redes de Computadores |
| Disciplina | Desenvolvimento Web I |
| Organização | [IFC Dev Web II](https://github.com/ifc-dev-web2) |

## Autoria

Projeto desenvolvido por **Nome do estudante** durante as atividades de
Desenvolvimento Web I.

Template elaborado pelo
[Prof. Cristofer Sousa](https://github.com/cristofersousa).

## Licença

Este projeto está disponível sob os termos definidos no arquivo
[LICENSE](./LICENSE).
