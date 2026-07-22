# VERSIONAMENTO
### A1 Game Academy

## Regras Gerais

- Commits por etapa concluída — evite commits gigantes que misturam
  várias mudanças não relacionadas.
- Documentação e código evoluem juntos: se uma mudança de código torna
  um documento desatualizado, o documento é corrigido no mesmo ciclo
  de trabalho (ver Seção 8 do `METODOLOGIA.md`).
- Versionamento semântico quando aplicável (ex: releases do jogo).

---

## Estratégia de Branches

Cada Sprint é desenvolvida em sua própria branch, criada a partir da `main`.

**Convenção de nome:**
```
sprint-XXX-nome-curto
```
Exemplo: `sprint-005-hordes-internas`

**Fluxo:**
1. Criar a branch no início da Sprint: `git checkout -b sprint-005-hordes-internas`
2. Trabalhar e commitar normalmente dentro dela.
3. Quando a Sprint for concluída e testada, fazer merge de volta na `main`.
4. A branch pode ser apagada após o merge (o histórico permanece preservado
   nos commits da `main`).

A `main` deve, na medida do possível, representar sempre uma versão
funcional do jogo.

---

## Convenção de Commits (Conventional Commits)

Toda mensagem de commit segue o formato:

```
tipo: descrição curta no imperativo
```

**Tipos utilizados:**

| Tipo | Uso |
|---|---|
| `feat:` | Funcionalidade nova |
| `fix:` | Correção de bug |
| `refactor:` | Reorganização de código sem mudar comportamento |
| `docs:` | Mudança apenas de documentação |
| `chore:` | Tarefas administrativas (`.gitignore`, configs, dependências) |

**Exemplos:**
```
feat: adiciona sistema de horde interna
fix: corrige spawn sobrepondo área de colisão da porta
refactor: separa room_data de door_data
docs: atualiza VISAO.md para v2.0
chore: adiciona .venv ao gitignore
```

### Por que isso importa (além de organização)

O histórico de commits, seguindo essa convenção, vira automaticamente
um roteiro cronológico de features, bugs e decisões — útil tanto para
retomar o projeto quanto como material bruto para vídeos e cursos.

---

## Histórico de Versões

### v2.0
- Adicionada estratégia de branches (uma por Sprint).
- Adicionada convenção de commits (Conventional Commits), com os tipos
  feat/fix/refactor/docs/chore.

### v1.0
- Versão original, criada antes do início do desenvolvimento.
