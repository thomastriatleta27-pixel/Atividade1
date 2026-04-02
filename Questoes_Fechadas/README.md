# RELATÓRIO AUTOMATIZADO COM LLMS + CURADORIA (OAB BENCH) ⚖️

Projeto para processamento automatizado de questões **fechadas** da OAB utilizando Inteligência Artificial, com geração de XML estruturado e relatório analítico em PDF.

---

## 🔄 Visão Geral do Pipeline

O projeto segue uma sequência obrigatória de 3 etapas para garantir a integridade dos dados e a precisão do relatório:

```mermaid
graph TD
  A[inferencia_oab_questoes_fechadas.py] -->|Gera Inferência| B[gerar_relatorio_inferencia_fechado.py]
  B -->|Gera XML Estruturado| C[gerar_relatorio_pdf_fechado.py]
  C -->|Gera PDF Final| D[Relatório_Final.pdf]
