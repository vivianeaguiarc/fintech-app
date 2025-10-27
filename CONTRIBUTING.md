# 🤝 Guia de Contribuição – Fin-Tech Multitenancy

Obrigado por contribuir com o projeto **Fin-Tech Multitenancy** 💸  
Este documento descreve as diretrizes para manter o repositório limpo, consistente e padronizado.

---

## 🧱 Estrutura de Branches

O fluxo de trabalho segue o padrão **Git Flow Simplificado**:

| Tipo de Branch | Prefixo   | Uso                                                 |
| -------------- | --------- | --------------------------------------------------- |
| **Main**       | `main`    | Versão estável e pronta para deploy                 |
| **Develop**    | `develop` | Integração contínua e código em progresso           |
| **Feature**    | `feat/`   | Novas funcionalidades                               |
| **Fix**        | `fix/`    | Correções de bugs                                   |
| **Chore**      | `chore/`  | Tarefas de manutenção (configurações, dependências) |
| **Docs**       | `docs/`   | Atualizações de documentação                        |

🪄 Exemplo:

```bash
git checkout -b feat/create-transaction-endpoint
```

---

## 🧾 Convenção de Commits (Conventional Commits)

Siga o padrão de commits para manter o histórico limpo e gerar changelogs automáticos:

```
<tipo>(escopo): descrição breve
```

### Tipos principais:

| Tipo       | Descrição                                           |
| ---------- | --------------------------------------------------- |
| `feat`     | Nova funcionalidade                                 |
| `fix`      | Correção de bug                                     |
| `docs`     | Alteração em documentação                           |
| `style`    | Formatação, espaçamento, etc.                       |
| `refactor` | Refatoração sem alterar comportamento               |
| `perf`     | Melhoria de performance                             |
| `test`     | Adição ou correção de testes                        |
| `chore`    | Configuração, dependências ou tarefas de manutenção |

🧩 Exemplos:

```
feat(auth): implementa login via Keycloak
fix(reports): corrige geração de PDF
docs(readme): adiciona seção de arquitetura
chore(ci): adiciona workflow de build no GitHub Actions
```

---

## 🧠 Boas práticas

- Crie commits **pequenos e significativos**
- Use mensagens em **português ou inglês**, mas sempre padronizadas
- Abra **Pull Requests (PRs)** descritivos com:
  - Objetivo
  - Alterações principais
  - Prints (se aplicável)

---

## 🧪 Testes e Qualidade de Código

Antes de abrir uma PR:

```bash
npm run lint
npm run test
```

Use o **Husky + Lint-Staged + Commitlint** para garantir qualidade automática.

---

## 💬 Dúvidas e Contato

Se tiver dúvidas, entre em contato com:

**👩‍💻 Viviane Aguiar**  
📧 [vivianeaguiarc@outlook.com](mailto:vivianeaguiarc@outlook.com)  
🔗 [LinkedIn](https://www.linkedin.com/in/vivianeaguiar)

---

✨ Obrigada por contribuir!

> “Código limpo é aquele que parece ter sido escrito por alguém que se importava.”
