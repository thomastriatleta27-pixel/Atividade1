# Curadoria de Dados - Exame da OAB ⚖️

Este repositório contém o trabalho de curadoria, classificação e processamento de questões do Exame da Ordem dos Advogados do Brasil (OAB), realizado como parte das atividades do **Grupo 01**.

## 🚀 Objetivo
Processar lotes de questões utilizando múltiplos modelos de Linguagem de Grande Escala (LLMs) para garantir a precisão na classificação e análise jurídica.

## 📂 Estrutura de Arquivos

### 📝 Questões Abertas (Lote 11 a 20)
Filtro das questões em dois formatos:
* `lote__abertas_thomas_oab_benc-11-20.xml`: Dados estruturados em XML.
* `lote__abertas_thomas_oab_benc-11-20.xml.csv`: Exportação dos resultados em formato CSV.

### 🔒 Questões Fechadas (Lote 107 a 212)
Filtro das questões em dois formatos:
* `lote_thomas_oab_bec_fechadas_107__a_212.xml`: Dados estruturados em XML.
* `lote__fecahdas_thomas_oab_benc-107_a_212.csv`: Exportação dos resultados em formato CSV.

## ⚖️ Metodologia de Curadoria

A classificação foi baseada em dois eixos principais:

### 📊 Nível de Dificuldade (Atribuído)
1. **Nível 1 - Estagiário:** Questões de aplicação direta da lei (literalidade).
2. **Nível 2 - Analista:** Questões que exigem conhecimento de ritos processuais ou prazos.
3. **Nível 3 - Juiz de Direito:** Questões que exigem interpretação de casos práticos e subsunção do fato à norma.
4. **Nível 4 - Ministro (STF/STJ):** Questões complexas envolvendo controle de constitucionalidade, súmulas vinculantes ou conflitos de leis.

### 📚 Áreas de Especialidade
As questões foram categorizadas conforme o dataset original e refinamento:
* Direito Constitucional
* Direito Penal
* Direito Administrativo
* Direito do Trabalho
* Direito Digital

* `ADIDIONAR DESCRICAO
*  ADIDIONAR DESCRICAO
  
---

## 🛠️ Tecnologias Utilizadas
* **Linguagem:** Python 3.x
* **Modelos de IA:** * Meta **Llama 3.3 70B** Versatile (via Groq)
    * Meta **Llama 3.1 8B** Instant (via Groq)
    * Alibaba **Qwen 2.5 7B** (via Hugging Face)
* **Bibliotecas:** `pandas`, `groq`, `huggingface_hub`, `datasets`, `fpdf`.

## 🧑‍💻 Autor
**Thomás Araujo** 
