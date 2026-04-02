# RELATÓRIO AUTOMATIZADO COM LLMS + CURADORIA (OAB BENCH) ⚖️

Projeto focado no processamento automatizado de questões **fechadas** da OAB utilizando Inteligência Artificial, com geração de base XML e relatório analítico final em PDF.

---

## 🔄 Visão Geral do Pipeline

O fluxo de trabalho é dividido em duas execuções obrigatórias:

1. **Código 01:** `gerar_relatorio_inferencia_fechado.py` (Processamento e Inferência)
2. **Código 02:** `gerar_relatorio_pdf_fechado.py` (Análise de Métricas e PDF)

**Fluxo:**
[Dataset] → [IA (LLAMA 3.1 8B)] → [Validação JSON] → [Gerar XML] → [Gerar PDF Final]

---

## 🛠️ Tecnologias Utilizadas

* **Python** (Pandas, LXML)
* **Groq API** (Modelo LLAMA 3.1 8B)
* **Hugging Face Datasets** (`eduagarcia/oab_exams`)
* **ReportLab** (Geração de PDF)

---

## 🚀 Como Executar no Google Colab

### 1️⃣ ETAPA 1 - Inferência e Geração de XML
Execute o primeiro código: **`gerar_relatorio_inferencia_fechado.py`**

* **Instalação:** `!pip install reportlab pandas groq datasets`
* **O que faz:** * Carrega as questões fechadas (Lote 107 a 212).
    * A IA atua como curadora, extraindo Área do Direito, Nível e Referência Legal.
    * Compara a resposta da IA com o gabarito oficial.
* **Resultado:** Gera o arquivo `curadoria_thomas.xml`.

### 2️⃣ ETAPA 2 - Relatório de Performance
Execute o segundo código: **`gerar_relatorio_pdf_fechado.py`** (ou script de relatório correspondente)

* **Dependência:** Requer o arquivo `curadoria_thomas.xml` gerado na etapa anterior.
* **O que faz:** * Lê os dados estruturados do XML.
    * Calcula métricas de Precisão (%), Total de Acertos e Erros.
    * Gera um relatório visual profissional.
* **Resultado:** Gera o arquivo `Relatorio_Thomas_Final_XML.pdf`.

---

## ⚖️ Metodologia de Curadoria

As questões são classificadas automaticamente nos seguintes níveis:
* **Nível 1 - Estagiário:** Aplicação direta da lei.
* **Nível 2 - Analista:** Ritos processuais e prazos.
* **Nível 3 - Juiz de Direito:** Interpretação de casos práticos.
* **Nível 4 - Ministro (STF/STJ):** Complexidade constitucional e súmulas.

---

## 📊 Estrutura dos Dados (XML)
Cada nó do arquivo contém:
* **ID / Enunciado / Área**
* **Resposta da IA vs. Gabarito Oficial**
* **Validação Automática (CORRETO/INCORRETO)**
* **Nível de Dificuldade e Base Legal**

---

## 🧑‍💻 Autor
**Thomás Araujo**
*NOC Assistant | Grupo 01 - Curadoria OAB*

> **Nota:** Mantenha suas chaves de API seguras e nunca as publique em repositórios públicos.
