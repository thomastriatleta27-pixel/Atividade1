🚀 Objetivo
Processar lotes de questões utilizando múltiplos modelos de Linguagem de Grande Escala (LLMs) para garantir a precisão na classificação e análise jurídica, seguido de curadoria humana especializada.

📂 Estrutura de Arquivos
📝 Questões Abertas (Lote 11 a 20)
Filtro das questões em dois formatos:

lote__abertas_thomas_oab_benc-11-20.xml: Dados estruturados em XML.

lote__abertas_thomas_oab_benc-11-20.xml.csv: Exportação dos resultados em formato CSV.

🔒 Questões Fechadas (Lote 107 a 212)
Filtro das questões em dois formatos:

lote_thomas_oab_bec_fechadas_107__a_212.xml: Dados estruturados em XML.

lote__fecahdas_thomas_oab_benc-107_a_212.csv: Exportação dos resultados em formato CSV.

📊 Curadoria Analítica (Excel)
Classificação manual baseada em nível de dificuldade e área:

Questões Abertas: Curadoria_questoes_abertas_thomas_11_a_20.xlsx

Questões Fechadas: Curadoria_questoes_fechadas_thomas_107_a_212.xlsx

📚 Relatórios de Inferência
Documentos consolidados com as respostas geradas pelas IAs:

Questões Abertas: Relatorio_Thomas_Final_Questoes_Abertas_11_20.pdf

Questões Fechadas: Relatorio_Thomas_Final_Questoes_fechadas_107_212.pdf

⚖️ Metodologia de Curadoria
📈 Níveis de Dificuldade
Nível 1 - Estagiário: Questões de aplicação direta da lei (literalidade).

Nível 2 - Analista: Questões que exigem conhecimento de ritos processuais ou prazos.

Nível 3 - Juiz de Direito: Questões que exigem interpretação de casos práticos e subsunção do fato à norma.

Nível 4 - Ministro (STF/STJ): Questões complexas envolvendo controle de constitucionalidade ou súmulas vinculantes.

📚 Áreas de Especialidade
Direito Constitucional / Penal / Administrativo / Trabalho / Digital.

🛠️ Tecnologias Utilizadas
Linguagem: Python 3.x

Modelos de IA: * Meta Llama 3.3 70B Versatile (via Groq)

Meta Llama 3.1 8B Instant (via Groq)

Alibaba Qwen 2.5 7B (via Hugging Face)

Bibliotecas: pandas, groq, huggingface_hub, datasets, fpdf.

🧑‍💻 Autor
Thomás Araujo
