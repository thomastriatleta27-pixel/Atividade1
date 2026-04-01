RELATÓRIO AUTOMATIZADO COM LLMS (OAB BENCH)

Este projeto utiliza múltiplos modelos de IA para responder questões abertas do dataset OAB Bench, gerando automaticamente um relatório em PDF com as respostas.

---

TECNOLOGIAS UTILIZADAS

* Groq API (LLAMA 3.3 70B e 3.1 8B)
* Hugging Face (Qwen 2.5)
* Google Colab
* Python
* FPDF (geração de PDF)

---

DATASET

Utilizado dataset público:
maritaca-ai/oab-bench

---

COMO EXECUTAR NO GOOGLE COLAB

1. Acesse o Colab:
   https://colab.research.google.com/

---

2. Instale as dependências:

!pip install groq
!pip install fpdf
!pip install huggingface_hub datasets

---

3. Configure suas chaves de API:

CHAVE_GROQ = "SUA_CHAVE_GROQ"
CHAVE_HF   = "SUA_CHAVE_HF"

IMPORTANTE:
Nunca compartilhe suas chaves publicamente.

---

4. Execute o código

Rode todas as células do notebook.

O script irá:

* Carregar o dataset
* Processar as questões
* Consultar 3 modelos de IA:

  * LLAMA 70B (alta qualidade)
  * LLAMA 8B (rápido)
  * Qwen 2.5 (estável)
* Gerar um relatório final em PDF

---

SAÍDA

Arquivo gerado:
Relatorio_Thomas_Lote_11_20.pdf

Para baixar no Colab:

from google.colab import files
files.download("Relatorio_Thomas_Lote_11_20.pdf")

---

ESTRUTURA DO PROJETO

* Entrada: questões abertas da OAB
* Processamento: múltiplas LLMs
* Saída: PDF comparativo com respostas

---

POSSÍVEIS PROBLEMAS

Erro 400 (Groq):

* Pode ser limite de requisição
* Tente usar time.sleep(2)

Erro Hugging Face:

* Verifique permissões da chave
* Alguns modelos exigem aceite de termos

PDF com caracteres estranhos:

* Limitação do encoding latin-1
* Já tratado com função limpar()

---

MELHORIAS FUTURAS

* Avaliação automática das respostas
* Integração com banco de dados
* Dashboard com resultados
* Uso de embeddings para análise semântica

---

AUTOR

Thomas Araujo

---

OBSERVAÇÃO

Projeto voltado para pesquisa e experimentação com modelos de linguagem aplicados ao Direito.

---
