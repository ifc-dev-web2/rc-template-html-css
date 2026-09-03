# Template HTML e CSS

Template inicial para projetos de Desenvolvimento Web do IFC desenvolvidos
apenas com HTML e CSS.

## Objetivo

Fornecer uma estrutura comum de arquivos e configurações para que diferentes
projetos utilizem o mesmo padrão de organização e formatação.

Este repositório também pode ser utilizado como referência para professores,
estudantes e desenvolvedores que desejam criar seu próprio repositório-base.

## Tecnologias

- HTML5;
- CSS3;
- EditorConfig;
- Prettier;
- Visual Studio Code.

## Usar este template

Quando o repositório estiver configurado como um template no GitHub:

1. selecione `Use this template`;
2. escolha `Create a new repository`;
3. informe o nome do novo projeto;
4. clone o repositório criado;
5. abra a pasta completa no Visual Studio Code;
6. instale as extensões recomendadas;
7. substitua o conteúdo inicial pelo conteúdo do seu projeto.

> Um repositório criado a partir do template é independente do repositório
> original. Por isso, utilize `Use this template` em vez de criar um fork.

## Estrutura do projeto

```text
.
├── .vscode/
│   ├── extensions.json
│   └── settings.json
├── css/
│   └── global.css
├── docs/
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

> No diretório `img/`, o arquivo `.gitkeep` é necessário porque o Git não
> versiona diretórios vazios.

## Extensões recomendadas

### Necessária para a padronização

- [Prettier — Code formatter](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode)

### Opcionais

- [Material Icon Theme](https://marketplace.visualstudio.com/items?itemName=PKief.material-icon-theme);
- [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer).

O Prettier é responsável pela formatação do código. As demais extensões melhoram
a experiência pessoal durante o desenvolvimento.

---

## Criar seu próprio repositório-base

Caso tenha interesse em criar um template ou repositório-base para seus
projetos, siga as etapas abaixo.

### 1. Crie o arquivo `.editorconfig`

```ini
root = true

[*]
charset = utf-8
end_of_line = lf
insert_final_newline = true
indent_style = space
indent_size = 2
trim_trailing_whitespace = true
max_line_length = 80

[*.md]
trim_trailing_whitespace = false
```

O EditorConfig estabelece regras básicas que podem ser reconhecidas por
diferentes editores e ferramentas.

### 2. Crie o arquivo `.prettierrc.json`

```json
{
  "printWidth": 80,
  "tabWidth": 2,
  "useTabs": false,
  "singleAttributePerLine": true,
  "bracketSameLine": false,
  "semi": true,
  "singleQuote": true,
  "endOfLine": "lf"
}
```

Esse arquivo define as regras utilizadas pelo Prettier para organizar o código.

### 3. Crie o arquivo `.prettierignore`

```gitignore
node_modules/
dist/
build/
coverage/
*.min.css
*.min.js
```

Os arquivos e diretórios listados não serão formatados pelo Prettier.

### 4. Crie o arquivo `.vscode/extensions.json`

```json
{
  "recommendations": [
    "esbenp.prettier-vscode",
    "PKief.material-icon-theme",
    "ritwickdey.LiveServer"
  ]
}
```

Ao abrir o projeto, o Visual Studio Code poderá recomendar essas extensões.

### 5. Crie o arquivo `.vscode/settings.json`

```json
{
  "editor.tabSize": 2,
  "editor.insertSpaces": true,
  "editor.detectIndentation": false,
  "editor.formatOnSave": true,
  "editor.formatOnPaste": true,
  "editor.defaultFormatter": "esbenp.prettier-vscode",
  "editor.renderWhitespace": "boundary",
  "editor.renderControlCharacters": true,
  "editor.rulers": [80],
  "editor.guides.indentation": true,
  "editor.guides.highlightActiveIndentation": true,

  "[html]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },

  "[css]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },

  "[javascript]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  }
}
```

Essas configurações são aplicadas quando a pasta completa do projeto é aberta
no Visual Studio Code.

### 6. Crie o arquivo `.gitignore`

```gitignore
# Dependências
node_modules/

# Arquivos de build
dist/
build/

# Relatórios
coverage/

# Sistemas operacionais
.DS_Store
Thumbs.db

# Editores
*.swp
*.swo

# Variáveis de ambiente
.env
.env.*
!.env.example
```

A pasta `.vscode/` não deve ser ignorada, pois contém configurações
compartilhadas pelo projeto.

## Validar a configuração

Depois de criar os arquivos, verifique:

- [ ] O Prettier formatou os arquivos HTML e CSS;
- [ ] os atributos HTML foram organizados em linhas separadas;
- [ ] a indentação utiliza dois espaços;
- [ ] a régua aparece na coluna 80;
- [ ] os espaços utilizados na indentação estão visíveis;
- [ ] o Live Server conseguiu abrir a página;
- [ ] o Git reconheceu a pasta `.vscode/`;
- [ ] os arquivos de configuração aparecem no `git status`.

## Criar o primeiro commit

```bash
git add .
git commit -m "chore: cria template base para projetos HTML e CSS"
git push origin main
```

## Transformar o repositório em template

No GitHub, acesse:

```text
Settings → General → Template repository
```

Marque a opção `Template repository`.

Depois disso, o botão `Use this template` ficará disponível na página principal
do repositório.

## Padronização do código

As regras de formatação fazem parte do projeto e devem ser utilizadas por todos
os participantes.

Para entender a responsabilidade de cada arquivo, consulte o
[guia de padronização do código](./docs/guia-padronizacao-codigo.md).

## Licença

Este projeto está distribuído sob a licença MIT.
