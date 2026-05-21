# 🍻 Bootcamp Heineken & DIO: IA Aplicada a Vendas

<p align="center">
  <img src="https://img.shields.io/badge/Status-Em_Desenvolvimento-blue?style=for-the-badge&logo=github" alt="Status"/>
  <img src="https://img.shields.io/badge/Bootcamp-DIO_&_Heineken-008200?style=for-the-badge&logo=heineken" alt="Bootcamp"/>
  <img src="https://img.shields.io/badge/Tech-Engenharia_de_Prompts_&_LLMs-000000?style=for-the-badge&logo=openai" alt="Tech"/>
</p>

## 🎯 Visão Geral do Projeto

Repositório central para documentação e versionamento das soluções de Inteligência Artificial desenvolvidas durante o Bootcamp **Inteligência Artificial Aplicada a Vendas (Heineken/DIO)**. 

O foco deste portfólio é demonstrar a aplicação prática de **Modelos de Linguagem de Grande Escala (LLMs)** e **Sistemas RAG (Retrieval-Augmented Generation via NotebookLM)** para otimização de rotinas comerciais, análise de dados e estruturação de assistentes virtuais (Copilotos) voltados para o ciclo de vendas B2B e atendimento ao cliente.

---

## 📂 Trilha de Desafios e Entregáveis

| Módulo/Desafio | Tipo de Atividade | Link para a Pasta | Explicação na Página |
| :--- | :---: | :---: | :---: |
| **1. Simplificando Tarefas e Ganhando Foco** | `Desafio Criativo` | [📂 Aceder Pasta](./) | [👁️ Ver Detalhes](#desafio-1) |
| **2. Treinando uma IA de Aprendizagem** | `Projeto Prático` | [📂 Aceder Pasta](./Modulo_02_NotebookLM) | [👁️ Ver Detalhes](#desafio-2) |
| **3. Acelerando Produtividade com IA** | `Desafio Criativo` | [📂 Aceder Pasta](./Modulo_03_Produtividade_Pessoal) | [👁️ Ver Detalhes](#desafio-3) |
| **4. O Poder da Argumentação Comercial** | `Desafio Criativo` | [📂 Aceder Pasta](./Modulo_04_Argumentacao_Comercial) | [👁️ Ver Detalhes](#desafio-4) |
| **5. Copiloto de Vendas com IA** | `Projeto Final` | ⏳ Pendente | [👁️ Ver Detalhes](#desafio-5) |

---

## 🛠️ Entregas Detalhadas

<a id="desafio-1"></a>
### 📦 1. Simplificando Tarefas e Ganhando Foco com IA no Dia a Dia

**Objetivo:** Transformar dados não estruturados da rotina de vendas em um cronograma operacional de alta eficiência.  
**Arquitetura do Prompt:** `Persona` > `Context Injection` > `Constraints` > `Output Format`.

**System Prompt da Entrega 01:**
```text
[SYSTEM ROLE]
Atue como um Especialista em Produtividade e Gestão Comercial.

[OBJECTIVE]
Gere um cronograma diário detalhado de foco e prospecção de clientes para a equipe comercial de campo (composta por Val, Duda e Eva). O objetivo central é priorizar o atendimento presencial aos Pontos de Venda (PDVs) estratégicos e otimizar as janelas de negociação do portfólio Heineken.

[CONTEXT INJECTION]
A equipe possui um modelo de trabalho híbrido dinâmico: dividem o tempo entre visitas físicas a bares/restaurantes parceiros e o gerenciamento remoto de pedidos e follow-ups operacionais através do WhatsApp.

[CONSTRAINTS & OUTPUT FORMAT]
1. Apresente o resultado estritamente em um formato de tabela de horários.
2. Cada bloco de tempo deve conter tarefas específicas, acionáveis e de curta duração.
3. É estritamente proibido sugerir a adoção de novas ferramentas de software, CRMs ou plataformas complexas. Baseie-se apenas em gestão de tempo nativa.
4. Utilize linguagem pragmática, eliminando jargões corporativos teóricos.
```

---

<a id="desafio-2"></a>
### 📦 2. Treinando uma IA de Aprendizagem: Explore o Poder do NotebookLM

**Objetivo:** Implementação de arquitetura RAG utilizando curadoria de fontes de alta autoridade para análise preditiva e inteligência de mercado no ecossistema B2B.

**📚 Curadoria de Fontes Utilizadas (Sources)**
* **[McKinsey & Company]** [AI in B2B Sales: The new growth equation](https://www.mckinsey.com/capabilities/growth-marketing-and-sales/our-insights/ai-in-b2b-sales) *(Revolução do funil de vendas B2B via GenAI).*
* **[IBM]** [O que é Inteligência Artificial na Cadeia de Suprimentos?](https://www.ibm.com/br-pt/topics/supply-chain-ai) *(Previsão de demanda e Machine Learning na logística).*
* **[RD Station]** [Como usar Inteligência Artificial em Vendas](https://resultadosdigitais.com.br/vendas/inteligencia-artificial-em-vendas/) *(Estratégias práticas e automação comercial).*
* **[Google Cloud]** [AI and Machine Learning for Retail](https://cloud.google.com/solutions/retail) *(Modelagem preditiva de comportamento de consumo).*

**🧠 Engenharia de Prompts e Cicatrizes (Troubleshooting)**
* **Abordagem Incorreta (Prompt Genérico):** *"Resuma o uso de IA nas vendas."*
  * *Resultado:* Resposta superficial focada apenas em automação de e-mails, ignorando a cadeia logística das fontes.
* **Abordagem Correta (Prompt Estruturado com Guardrails):**
  * *"Atue como um Analista de Dados Sênior. Baseado EXCLUSIVAMENTE nas fontes da IBM e McKinsey, construa uma tabela listando 3 aplicações práticas de análise preditiva para vendas B2B e otimização de estoque. Para cada aplicação, cite o benefício financeiro e a fonte de origem exata da informação."*
  * *Resultado:* Resposta exata, restrita ao contexto e mapeada por notas de rodapé das fontes.

**📖 Miniguia Consolidado**
* **Previsão de Demanda (Forecasting):** Algoritmos que cruzam histórico de vendas com variáveis externas (clima, sazonalidade) para evitar a ruptura de estoque nos PDVs.
* **Hiper-Personalização B2B:** Identificação automatizada do momento ideal de recompra com base no comportamento de pedidos dos clientes comerciais.
* **Glossário RAG:** *Retrieval-Augmented Generation* — técnica que força a IA a consultar documentos específicos antes de gerar respostas, eliminando alucinações.

---

<a id="desafio-3"></a>
### 📦 3. Acelerando Sua Produtividade Pessoal com IA

**Objetivo:** Engenharia de prompt focada em gerenciamento de tempo tático para aceder a estudos técnicos e transição de carreira.

**🧩 Elementos do Prompt**
* **Intenção:** Gerar um plano semanal de gerenciamento de tempo (*Timeblocking*) para um profissional em transição para a área de Dados.
* **Injeção de Contexto:** Rotina híbrida que concilia trabalho formal, graduação em negócios e bootcamps de tecnologia com disponibilidade de 3 a 4 horas úteis à noite.
* **Guardrails (Restrições):** Proibir cronogramas utópicos ou exaustivos, aplicar blocos Pomodoro e exigir janelas obrigatórias de descanso para mitigar o esgotamento mental.

**💻 O Prompt Final Consolidado:**
```text
Quero que a IA gere um plano semanal de produtividade e gestão de tempo para um profissional em transição de carreira para Análise de Dados, com o objetivo de eliminar a sobrecarga mental e garantir blocos de foco absoluto para o desenvolvimento de projetos práticos e certificações. Considere o seguinte contexto: o profissional precisa conciliar o trabalho diário com a graduação em Gestão de Negócios e bootcamps de tecnologia, possuindo cerca de 3 a 4 horas livres à noite. O conteúdo deve ter formato de tabela de blocos de tempo (Timeblocking), aplicando a técnica Pomodoro para estudos de ferramentas como SQL, Python e Power BI. Evite metas irreais, conselhos genéricos de autoajuda, acúmulo de tarefas pesadas em um único dia e a ausência de pausas para descanso.
```

---

<a id="desafio-4"></a>
### 📦 4. Argumentação Comercial com IA

**Objetivo:** Desenvolvimento de matrizes de objeção e scripts de negociação (*Pitch* de Vendas) para a equipe de campo B2B utilizando IA Generativa.

**🧩 Elementos do Prompt**
* **Intenção:** Criar um roteiro prático de contorno de objeções para converter lojistas e bares resistentes a produtos premium do portfólio Heineken.
* **Injeção de Contexto:** Simulação de objeções reais do mercado (ex: "produto muito caro" ou "falta de espaço na geladeira").
* **Guardrails (Restrições):** Proibir tom de telemarketing engessado e respostas teóricas. O output deve ser uma matriz visual voltada para o uso rápido no "chão de loja".

**💻 O Prompt Final Consolidado:**
```text
Quero que a IA gere um roteiro prático de contorno de objeções e argumentação de vendas para a equipe comercial (Val, Duda e Eva), com o objetivo de treiná-las para converter lojistas e donos de bares que resistem à introdução de novos produtos premium do portfólio Heineken. Considere o seguinte contexto: os clientes geralmente alegam barreiras como 'a cerveja premium é muito cara para o público do meu bar' ou 'não tenho espaço livre na geladeira'. O conteúdo deve ter formato de matriz de objeções (Coluna 1: Objeção do Cliente -> Coluna 2: Gatilho de Persuasão -> Coluna 3: Resposta Prática para o vendedor falar no balcão). Evite argumentos engessados de telemarketing, agressividade comercial e respostas teóricas longas que não funcionam na vida real.
```

---

<a id="desafio-5"></a>
### 🚀 5. [PROJETO FINAL] Copiloto Especialista de Vendas

*Consolidação de todas as habilidades da trilha na construção de um agente autônomo (Copiloto) especializado no portfólio Heineken.*

> ⏳ **Status:** Aguardando início do desenvolvimento. O prompt mestre e a documentação do agente serão disponibilizados no fim do bootcamp.

---

## 👨‍💻 Autor

**Yugo Pereira** *Desenvolvendo soluções escaláveis na interseção entre Dados, Negócios e Inteligência Artificial.*

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/yugopereira/)
[![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/YugoPereira)
