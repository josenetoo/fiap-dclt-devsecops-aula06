# 📊 Relatórios de Exemplo

Esta pasta contém relatórios de exemplo para uso nas aulas 6.2 e 6.3.

## 📁 Arquivos Disponíveis

| Arquivo | Scanner | Vulnerabilidades |
|---------|---------|------------------|
| `horusec-results.json` | Horusec (SAST) | 5 findings (2 Critical, 2 High, 1 Medium) |
| `trivy-results.json` | Trivy (SCA/Container) | 8 CVEs (1 Critical, 4 High, 2 Medium, 1 Low) |
| `zap-results.json` | OWASP ZAP (DAST) | 6 findings (2 High, 1 Medium, 3 Low) |

## 🚀 Como Usar

### Upload via Interface Web (Recomendado)

> ℹ️ **DefectDojo Open Source**: O Import Scan é acessado via Engagement.

1. Acesse DefectDojo: http://localhost:8080
2. Login: `admin` / `admin123`
3. Menu lateral > **Engagements** > **All Engagements**
4. Clique no engagement `Pipeline CI/CD`
5. Clique em **Import Scan Results**
6. Selecione **Scan Type**: `Generic Findings Import`
7. Faça upload do arquivo (Choose):
   - `horusec-results.json` (SAST)
   - `trivy-results.json` (SCA)
   - `zap-results.json` (DAST)
8. Clique **Import**

> ⚠️ **Importante**: Use sempre `Generic Findings Import` como Scan Type para estes relatórios.

## 📋 Resumo das Vulnerabilidades

### Horusec (SAST)
- **CRITICAL**: API Key hardcoded, SQL Injection
- **HIGH**: Senha hardcoded, Uso de eval()
- **MEDIUM**: Logging de dados sensíveis

### Trivy (Container/SCA)
- **CRITICAL**: CVE-2021-44228 (Log4Shell)
- **HIGH**: CVE-2023-44487 (HTTP/2 Rapid Reset), CVE-2022-29458, CVE-2023-4911
- **MEDIUM**: CVE-2022-40674, CVE-2022-25883
- **LOW**: CVE-2021-33560, CVE-2024-4068

### ZAP (DAST)
- **HIGH**: XSS Reflected, SQL Injection
- **MEDIUM**: Missing Anti-clickjacking Header
- **LOW**: XSS Protection, HSTS, X-Content-Type-Options

## 🎯 Objetivo Pedagógico

Estes relatórios permitem:
1. Demonstrar upload para DefectDojo sem precisar executar scans reais
2. Visualizar diferentes severidades no Dashboard
3. Praticar triagem e gestão de vulnerabilidades
4. Configurar e testar SLAs
