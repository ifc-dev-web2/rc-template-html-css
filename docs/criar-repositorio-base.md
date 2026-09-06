# Como criar um repositório-base para HTML e CSS

Este guia apresenta os arquivos necessários para criar um template de projetos
HTML e CSS com configurações compartilhadas de formatação.

> Para entender detalhadamente a responsabilidade e o funcionamento de cada
> arquivo, consulte o [guia de padronização do código](./guia-padronizacao-codigo.md).

## 1. Crie o EditorConfig

Crie o arquivo `.editorconfig` na raiz do projeto:

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

## 2. Configure o Prettier

Crie o arquivo `.prettierrc.json`:

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

Depois, crie o arquivo `.prettierignore`:

```gitignore
node_modules/
dist/
build/
coverage/
*.min.css
*.min.js
```

## 3. Recomende as extensões do VS Code

Crie o diretório `.vscode/` e, dentro dele, o arquivo `extensions.json`:

```json
{
  "recommendations": [
    "esbenp.prettier-vscode",
    "PKief.material-icon-theme",
    "ritwickdey.LiveServer"
  ]
}
```

## 4. Compartilhe as configurações do editor

No diretório `.vscode/`, crie também o arquivo `settings.json`:

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

## 5. Configure o Git

Crie o arquivo `.gitignore`:

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

O diretório `.vscode/` não deve ser ignorado, pois contém configurações que
precisam acompanhar o projeto.

## 6. Valide a configuração

Antes de publicar o template, confira:

- [ ] o Prettier formata os arquivos HTML e CSS;
- [ ] os atributos HTML são organizados em linhas separadas;
- [ ] a indentação utiliza dois espaços;
- [ ] a régua aparece na coluna 80;
- [ ] o Live Server abre a página;
- [ ] o Git reconhece o diretório `.vscode/`;
- [ ] todos os arquivos de configuração aparecem no `git status`.

## 7. Crie o primeiro commit

```bash
git add .
git commit -m "chore: cria template base para projetos HTML e CSS"
git push origin main
```

## 8. Transforme o repositório em template

No GitHub, acesse:

```text
Settings → General → Template repository
```

Marque a opção **Template repository**. O botão **Use this template** ficará
disponível na página principal do repositório.
