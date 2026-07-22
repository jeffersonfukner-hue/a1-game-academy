# PADRÕES
### A1 Game Academy

## Nomenclatura de Arquivos

- Documentação institucional (metodologia, administração, padrões):
  nome em MAIÚSCULAS (ex: `METODOLOGIA.md`, `ROADMAP.md`).
- Arquivos de apresentação de repositório (ex: `README.md`): sempre
  como a convenção do GitHub exige, em maiúscula inicial apenas.
- Sprints: `SPRINT_XXX.md`, numeração sequencial de 3 dígitos.
- Documentos de projeto específico (não institucionais): livre, desde
  que consistente dentro do próprio repositório.

## Estrutura de Pastas

### Repositório institucional (`a1-game-academy`)
```
docs/
 ├── administracao/    → missão, roadmap, regras administrativas
 ├── metodologia/       → METODOLOGIA.md, VERSIONAMENTO.md, PADROES.md
 ├── infraestrutura/    → (reservado para uso futuro)
 ├── projetos/          → referências aos repositórios de cada jogo
 ├── recursos/          → (reservado para uso futuro)
 └── deprecated/         → documentos obsoletos deste repositório
```

### Repositório de projeto (ex: `forgotten-ship`)
```
docs/
 ├── VISAO.md
 ├── PROJETO.md
 ├── ROADMAP.md
 ├── sprints/
 │    ├── SPRINT_001.md, SPRINT_002.md, ...
 └── deprecated/         → documentos obsoletos deste repositório
```

## Documentos Obsoletos

Nenhum documento é apagado quando substituído — ele é movido para a
pasta `deprecated/` **na raiz de `docs/` de cada repositório** (um único
`deprecated/` por repositório, não uma pasta por subcategoria).
Isso preserva o histórico como material de aprendizado (inclusive para
vídeos/curso, mostrando a evolução real do processo).

## Um Projeto, Uma Documentação Própria

Cada jogo tem seu próprio repositório e sua própria pasta `docs/`,
independente da documentação institucional da Academia. A Academia
referencia os projetos, mas não duplica seu conteúdo.

## Histórico de Versões

### v2.1
- Corrigido: um único `deprecated/` por repositório (raiz de `docs/`),
  não uma subpasta por categoria — ajustado para bater com a estrutura
  real adotada na prática.

### v2.0
- Reescrito para refletir a estrutura de pastas e a convenção
  `deprecated/` já em uso, consolidando regras que existiam apenas
  na prática, não em documento.

### v1.0
- Versão original, criada antes do início do desenvolvimento.
