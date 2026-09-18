# Projects_MetaAcademy

## Fluxo de Trabalho no GitHub & Deploy com GitHub Pages

Este repositório documenta a execução prática do fluxo de trabalho essencial no Git e GitHub, abrangendo a configuração do ambiente local, gestão de branches, criação de arquivos de configuração, publicação de páginas estáticas via GitHub Pages e abertura de Pull Requests.

---

## 🛠️ Tecnologias e Ferramentas Utilizadas

- **Git**: Controle de versionamento de código.
- **GitHub**: Hospedagem do repositório remoto e serviço de hospedagem (GitHub Pages).
- **VS Code**: Editor de código-fonte.
- **HTML5**: Estrutura básica da página web.

---

## 📝 Passo a Passo das Atividades Realizadas

### 1. Configuração do Ambiente e Clonagem
1. Criada a pasta de trabalho `projects` no ambiente local.
2. Criado o repositório no GitHub.
3. Clonado o repositório remoto para a máquina local via terminal:
   ```bash
   git clone <URL-DO-SEU-REPOSITORIO>
    ```
  ### 2. Configuração do `.gitignore`

1. Projeto aberto no VS Code.
2. Criado o arquivo `.gitignore` para ignorar diretórios de configurações locais de IDEs:
````snippet de código
.idea
.vscode
````
3. Salvas e enviadas as alterações para a branch principal (`main`):

````bash
git status
git add .gitignore
git commit -m ".gitignore was added"
git push origin main
````
### 3. Criação da Branch e Desenvolvimento da Página

Criada e ativada a nova branch `gh-pages`:
````bash
git branch gh-pages
git checkout gh-pages
````

Criado o arquivo `index.html` com o conteúdo:
````html
<h1>Hello world!</h1>
````
Realizado o commit e envio da branch para o GitHub:
````bash
git add index.html
git commit -m "create index.html"
git push origin gh-pages
````
### 4. Deploy no GitHub Pages
1. Nas configurações do repositório no GitHub (Settings > Pages), definiu-se a branch `gh-pages `como fonte de publicação (Source).
2. O site foi publicado com sucesso.

## 🔀 Pull Request (PR)

Foi aberta uma Pull Request no GitHub comparando as alterações:

 - Base branch: `main` 

 - Compare branch: `gh-pages`

A PR inclui a verificação do arquivo `index.html` alterado e o link para validação da página pública enviada.
