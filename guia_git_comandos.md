
# ✅ Guia Essencial de Comandos Git + Bash

## 📦 Instalação do Git (Linux)
```bash
$ sudo apt-get update
$ sudo apt-get install git
```

## ⚙️ Configuração Inicial do Git
```bash
$ git version                            # Verifica a versão instalada
$ git config --global user.name "Seu Nome"      # Define seu nome globalmente
$ git config --global user.email "email@dom.com" # Define seu e-mail globalmente
$ git config user.name                  # Mostra nome configurado
$ git config user.email                 # Mostra e-mail configurado
$ git config --global core.editor "caminho/editor" # Define editor padrão
$ git config core.editor                # Mostra editor configurado
```

## 💻 Comandos Básicos do Terminal Bash
```bash
$ clear               # Limpa o terminal
$ pwd                 # Mostra diretório atual
$ cd nome_pasta       # Entra em uma pasta
$ cd ..               # Sobe um nível
$ ls                  # Lista arquivos e pastas
$ mkdir nome_pasta    # Cria uma pasta
$ touch nome.txt      # Cria um arquivo
$ touch pasta/arquivo.txt # Cria arquivo dentro da pasta
```

## 🔧 Iniciando um Repositório Git
```bash
$ git init            # Inicia um repositório Git (cria .git)
$ git status          # Mostra status dos arquivos
$ git add .           # Adiciona todas as mudanças
$ git add nome.ext    # Adiciona arquivo específico
$ git reset HEAD nome.ext # Remove do stage
$ git commit -m "mensagem" # Cria um commit
$ git commit -am "msg"     # Add + commit (sem git add explícito)
```

## 📜 Histórico e Visualização de Commits
```bash
$ git log             # Histórico detalhado
$ git log --oneline   # Resumo dos commits
$ git log --graph     # Visual gráfico dos commits
$ git log --graph --oneline --all  # Todos os commits visualmente
$ git diff            # Diferenças antes de um commit
```

## 🌿 Branches (Ramificações)
```bash
$ git branch                   # Lista branches
$ git branch nome_ramo         # Cria novo ramo
$ git checkout nome_ramo       # Muda para o ramo
$ git checkout -b nome_ramo    # Cria e muda para novo ramo
$ git merge nome_ramo          # Une ramo com branch atual
$ git merge --abort            # Aborta merge em conflito
$ git checkout master          # Retorna à branch principal
```

## 🧭 Navegação entre versões
```bash
$ git checkout <hash>          # Volta a um commit anterior
$ git reset --hard <hash>      # Remove commits posteriores ao hash
$ git checkout nome.ext        # Reverte alterações de um arquivo
```

## 🌐 Repositório Remoto
```bash
$ git remote                   # Verifica repositórios remotos
$ git remote -v                # Lista URLs remotas
$ git remote add origin https://github.com/usuario/repositorio.git  # Conecta ao remoto
$ git push -u origin master    # Envia commits locais ao GitHub
$ git pull                     # Atualiza repositório local com o remoto
$ git fetch                    # Baixa alterações (sem merge automático)
```

## 🔁 Clonar Repositórios
```bash
$ git clone https://github.com/usuario/repositorio.git
```

## 🔑 Token de Acesso (HTTPS com autenticação)
- Gere em: [https://github.com/settings/apps](https://github.com/settings/apps)

## 📂 Trabalhando com Forks e Pull Requests
- **Fork:** Cópia de um repositório para alterações sem afetar o original.
- **Pull Request:** Solicitação para integrar suas alterações ao projeto original.
- **Issues:** Área para reportar bugs, sugerir melhorias ou iniciar discussões.

## 📝 Dicas Finais
- Use `code .` (com VS Code instalado e configurado) para abrir o projeto diretamente no editor.
- Use `git stash` para guardar temporariamente alterações sem commitar.
- Use `git rebase` (com cuidado) para reescrever histórico de commits.
