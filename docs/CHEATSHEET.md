# Aula 06 - DefectDojo Cheatsheet

## Docker Compose

```bash
cd defectdojo
docker-compose up -d
docker-compose logs -f initializer
```

## Credenciais Padrão

- URL: http://localhost:8080
- User: admin
- Pass: admin123

## API Upload

```bash
curl -X POST "${URL}/api/v2/import-scan/" \
  -H "Authorization: Token ${API_KEY}" \
  -F "scan_type=Trivy Scan" \
  -F "file=@report.json" \
  -F "engagement=${ENGAGEMENT_ID}"
```

## Scan Types

| Scanner | Tipo |
|---------|------|
| Trivy | `Trivy Scan` |
| Horusec | `Horusec Scan` |
| ZAP | `ZAP Scan` |
| SARIF | `SARIF` |

## CVSS Scores

| Score | Severidade | SLA |
|-------|------------|-----|
| 9.0-10.0 | Critical | 24h |
| 7.0-8.9 | High | 7 dias |
| 4.0-6.9 | Medium | 30 dias |
| 0.1-3.9 | Low | 90 dias |

## Hierarquia

```
Product Type → Product → Engagement → Test → Finding
```
