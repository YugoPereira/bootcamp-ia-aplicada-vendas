# 📓 Desafio 02: Treinando uma IA de Aprendizagem com NotebookLM

<p align="center">
  <img src="https://img.shields.io/badge/Ferramenta-NotebookLM-blue?style=for-the-badge&logo=google" alt="Ferramenta"/>
  <img src="https://img.shields.io/badge/Foco-RAG_&_Curadoria_de_Dados-008200?style=for-the-badge" alt="Foco"/>
  <img src="https://img.shields.io/badge/Status-Concluído-success?style=for-the-badge" alt="Status"/>
</p>

## 🎯 Contexto e Objetivos

Este projeto explora o poder da curadoria de dados e do framework RAG (*Retrieval-Augmented Generation*) utilizando o Google NotebookLM. 

**Tema do Caderno Temático:** Aplicação de IA e Análise Preditiva na Gestão de Vendas B2B e Previsão de Demanda.

**Objetivos de Estudo:**
1. Compreender como a IA pode prever a demanda de produtos e otimizar o estoque.
2. Mapear estratégias de prospecção e relacionamento no setor B2B.
3. Testar a capacidade do NotebookLM de cruzar informações entre artigos técnicos, vídeos e relatórios de mercado, extraindo apenas insights baseados nas fontes.

---

## 📚 Curadoria de Fontes (Sources)

Para construir o "cérebro" deste caderno e garantir respostas de alto nível comercial e técnico, selecionei fontes reais que combinam teoria de IA com aplicação prática no mercado:

1. **[Relatório de Mercado / McKinsey & Company]** [AI in B2B Sales: The new growth equation](https://www.mckinsey.com/capabilities/growth-marketing-and-sales/our-insights/ai-in-b2b-sales) *(Como grandes empresas estão usando IA generativa para revolucionar o funil de vendas B2B).*
2. **[Artigo Técnico / IBM]** [O que é Inteligência Artificial na Cadeia de Suprimentos?](https://www.ibm.com/br-pt/topics/supply-chain-ai) *(Conceitos de Machine Learning na logística e previsão de demanda de produtos).*
3. **[Guia Prático / RD Station]** [Como usar Inteligência Artificial em Vendas](https://resultadosdigitais.com.br/vendas/inteligencia-artificial-em-vendas/) *(Estratégias práticas, ferramentas e automação para equipes comerciais).*
4. **[Vídeo / Google Cloud]** [AI and Machine Learning for Retail](https://cloud.google.com/solutions/retail) *(Soluções visuais e conceitos de como a nuvem e a IA prevêem o comportamento de compra em escala).*

---

## 🧠 Engenharia de Prompts e "Cicatrizes" (Troubleshooting)

Nesta etapa, registrei o processo iterativo de testes com a IA, demonstrando como o refinamento do prompt muda drasticamente a qualidade da resposta.

### ❌ Teste 1: Prompt Amplo (O Erro)
* **Prompt:** *"Resuma o que os documentos falam sobre o uso de IA nas vendas."*
* **Resultado:** A IA gerou um resumo muito genérico, focando apenas em "escrever e-mails mais rápido" (baseado superficialmente no guia da RD Station), perdendo a profundidade analítica dos materiais da IBM e McKinsey.
* **Cicatriz/Troubleshooting:** Aprendi que prompts genéricos fazem o NotebookLM nivelar a resposta por baixo. É preciso direcionar o "foco de leitura" e exigir o cruzamento das fontes.

### ⚠️ Teste 2: Prompt Específico, mas sem Restrição
* **Prompt:** *"Liste aplicações práticas de IA na previsão de demanda e gestão de estoque."*
* **Resultado:** A IA trouxe boas aplicações, mas incluiu exemplos externos que ela já conhecia sobre empresas de tecnologia, fugindo do contexto dos documentos fornecidos.
* **Cicatriz/Troubleshooting:** O NotebookLM usou seu conhecimento prévio (fora do RAG). Precisei aplicar uma restrição rigorosa (*Guardrail*) para forçá-lo a usar apenas as URLs e PDFs anexados.

### ✅ Teste 3: Prompt Engenharizado (O Acerto)
* **Prompt Final:** *"Atue como um Analista de Dados Sênior. Baseado EXCLUSIVAMENTE nas fontes da IBM e McKinsey, construa uma tabela listando 3 aplicações práticas de análise preditiva para vendas B2B e otimização de estoque. Para cada aplicação, cite o benefício financeiro e a fonte de origem exata da informação."*
* **Resultado:** Resposta cirúrgica, formatada em tabela, sem alucinações e com citação exata (footnotes) apontando exatamente para os parágrafos corretos dos artigos fornecidos.

---

## 📖 Miniguia de Estudo: Inteligência de Vendas B2B

Abaixo, o material consolidado gerado pela interação otimizada com o NotebookLM.

### 1. Resumo Estruturado do Assunto
A integração da IA nas vendas B2B atua em três pilares fundamentais de rentabilidade:
* **Previsão de Demanda (Forecasting):** A IA analisa dados históricos, sazonalidade e variáveis externas para sugerir a quantidade exata de abastecimento, evitando ruptura ou excesso de estoque (baseado no artigo da IBM).
* **Hiper-Personalização B2B:** Modelos preditivos identificam o momento ideal de recompra e geram recomendações de produtos específicas para cada perfil de cliente, aumentando o ticket médio (insights do relatório McKinsey).
* **Eficiência da Força de Vendas:** Automação de tarefas repetitivas de CRM e geração de scripts de abordagem, permitindo que a equipe comercial passe mais tempo negociando e menos tempo em trabalhos administrativos (Guia RD Station).

### 2. Glossário Técnico
* **Análise Preditiva:** Uso de dados históricos e Machine Learning para prever comportamentos futuros de compra.
* **Supply Chain (Cadeia de Suprimentos):** Todo o fluxo logístico e de dados desde a fabricação do produto até a entrega no Ponto de Venda (PDV).
* **RAG (Retrieval-Augmented Generation):** Técnica onde a IA consulta uma base de conhecimento específica (nossas 4 fontes) antes de gerar a resposta, garantindo precisão e evitando invenções.
* **Ruptura de Estoque:** Quando um cliente deseja comprar um produto, mas ele está em falta devido a erros de previsão de demanda.

### 3. Prompts Reutilizáveis para Revisão
Guarde estes prompts para usar no seu Caderno do NotebookLM sempre que quiser testar seu conhecimento:
* 🔄 *"Gere um quiz de 5 perguntas de múltipla escolha baseado no Glossário destas fontes. Diga a resposta correta e a explicação apenas depois que eu responder."*
* 🔄 *"Atue como um comprador corporativo cético sobre a digitalização. Crie um diálogo onde eu (vendedor) preciso usar os argumentos do artigo da McKinsey para convencê-lo."*
* 🔄 *"Crie um resumo executivo de 2 parágrafos combinando o conceito de logística da IBM com as táticas de vendas da RD Station."*

---

## 👨‍💻 Autor
**Yugo Pereira**  
*Desenvolvido durante o Bootcamp IA Aplicada a Vendas (Heineken | DIO)*
