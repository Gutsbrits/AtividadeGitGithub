# AtividadeGitGithub
Atividade em grupo para colocar em prática os passos necessários para o versionamento de um projeto.

# ✅ Atividade Prática – Git & GitHub em Grupos  

## 👥 Papéis
- [ ] **DEV A** → Revisar/mesclar PRs e criar tags  
- [ ] **DEV B** → Criar novas features e corrigir bugs  
- [ ] **DEV C** → Auxiliar em features e resolver conflitos  

---

## 📌 Passo a Passo

### 1. Criação do repositório
- [ ] DEV A cria repositório **privado** no GitHub com README  
- [ ] DEV B e DEV C fazem `git clone`  
- [ ] Todos configuram Git local (`user.name` e `user.email`)  

### 2. Configuração inicial
- [ ] Criar arquivo `.env` com variáveis de ambiente  
- [ ] Criar `.gitignore` incluindo `.env`  
- [ ] `git add . && git commit -m "Configuração inicial"`  
- [ ] Push para `main`  

### 3. Estrutura de Branches
- [ ] DEV A cria a branch `develop`  
- [ ] Fazer push da `develop` para o GitHub  

### 4. Simulação de Features
- [ ] DEV B cria branch `feature/...` a partir de `develop`  
- [ ] DEV C cria branch `feature/...` a partir de `develop`  
- [ ] Cada um cria/edita arquivo, faz commit e push  
- [ ] Abrir Pull Request → alvo `develop`  

### 5. Revisão e Merge
- [ ] DEV A revisa PRs no GitHub  
- [ ] DEV A faz merge das features na `develop`  

### 6. Correções (Bugfix & Hotfix)
- [ ] Criar `bugfix/...` a partir da `develop` → corrigir e abrir PR para `develop`  
- [ ] Criar `hotfix/...` a partir da `main` → corrigir e abrir PR para `main`  

### 7. Uso do Git Stash
- [ ] Um dev inicia alteração em `index.html`  
- [ ] Executa `git stash save "descrição"`  
- [ ] Troca de branch e depois recupera com `git stash pop`  

### 8. Criação de Versões
- [ ] Após merges na `main`, DEV A cria tag:  
  ```bash
  git tag -a v1.0.0 -m "Versão 1.0.0 estável"
  git push origin v1.0.0