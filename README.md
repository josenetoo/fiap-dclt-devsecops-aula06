# Aula 06 - Centralização com DefectDojo

## 🎯 Objetivo

Centralizar todas as vulnerabilidades em uma plataforma única usando DefectDojo.

## Vídeos desta Aula

| Vídeo | Tema | O que você vai fazer |
|-------|------|---------------------|
| 01 | Setup DefectDojo | Subir via Docker, criar produtos |
| 02 | Ingestão de Dados | Upload de reports via interface e API |
| 03 | Métricas e SLAs | Dashboard, CVSS, priorização |

## Estrutura do Repositório

```
.
├── defectdojo/
│   └── docker-compose.yml  # Setup do DefectDojo
├── sample-reports/         # Relatórios de exemplo para demonstração
│   ├── horusec-results.json
│   ├── trivy-results.json
│   └── zap-results.json
└── docs/
    └── HANDS-ON-06-*.md
```

## Pré-requisitos

- [ ] Aula 05 concluída
- [ ] Docker instalado (4GB+ RAM)
- [ ] Relatórios de scans (incluídos em `sample-reports/`)

## 📚 Documentação

| Vídeo | Hands-on |
|-------|----------|
| 01 - Setup DefectDojo | [HANDS-ON-06-01.md](docs/HANDS-ON-06-01.md) |
| 02 - Ingestão de Dados | [HANDS-ON-06-02.md](docs/HANDS-ON-06-02.md) |
| 03 - Métricas e SLAs | [HANDS-ON-06-03.md](docs/HANDS-ON-06-03.md) |

**Referência rápida**: [Cheatsheet](docs/CHEATSHEET.md)

---

**FIAP - Pós Tech DevSecOps**
