# 🛋️ Especialista em Precificação de Higienização de Estofados com IA

**Autor:** Thiago Sérgio  
**Tecnologia Utilizada:** Google NotebookLM, Engenharia de Prompts  

---

## 🎯 Contexto e Objetivos

Precificar corretamente os serviços de higienização de estofados (residenciais e automotivos) é um dos maiores desafios para quem atua na área. Cobrar um valor muito baixo atrai prejuízo, e cobrar sem critério afasta clientes. 

Este projeto nasceu da necessidade de criar um **Especialista de Precificação** inteligente, utilizando o NotebookLM do Google. O objetivo deste caderno temático e miniguia de estudos é:
1. Mapear custos fixos e variáveis de uma operação de limpeza de estofados.
2. Entender a diferença de precificação entre serviços residenciais (sofás, colchões) e estética automotiva (bancos, tetos).
3. Utilizar Inteligência Artificial para analisar o mercado, formatar combos de serviços e calcular o valor da hora técnica.

---

## 📚 Curadoria de Fontes

Para treinar o NotebookLM e criar uma base de conhecimento sólida e livre de "alucinações", foram selecionados materiais em texto e transcrições de especialistas do setor. As fontes utilizadas (disponibilizadas no repositório) incluem:

1. **Como Precificar Limpeza de Estofados e LUCRAR de Verdade!** (Foco em custos fixos, variáveis e valor da hora de trabalho).
2. **Qual o Valor de cada Serviço de Limpeza de Estofado?** (Foco em tabelas de preços médios, como sofás a R$180, colchões de casal a R$200, bancos de carro a R$150-R$180).
3. **LIVE LP: COMO COBRAR O SERVIÇO DE LIMPEZA DE ESTOFADOS?** (Foco em técnicas de vendas, combos e atendimento ao cliente).
4. **Limpeza de estofados VALE A PENA PARA 2025?** (Análise de mercado, projeção de faturamento e margem de lucro de até 70%).

---

## 🛠️ Engenharia de Prompts e "Cicatrizes" (Troubleshooting)

Ao interagir com o NotebookLM, testei diversas abordagens para extrair o melhor método de precificação. Abaixo está o registro dessa evolução:

### ❌ Tentativa 1 (Muito amplo)
* **Prompt:** *"Como devo cobrar para limpar um sofá e um carro?"*
* **Resultado:** A IA deu uma resposta genérica, sugerindo apenas "pesquisar a concorrência e somar os custos", sem apresentar valores ou métricas reais das fontes.

### ⚠️ Tentativa 2 (Ajustando o contexto)
* **Prompt:** *"Quais são os valores médios cobrados por serviços de higienização segundo as fontes, e quais custos devo considerar?"*
* **Resultado:** A IA listou os valores (ex: R$180 para sofá de 3 lugares), mas misturou custos fixos da empresa com o custo de produto por serviço.
* **Cicatriz/Troubleshooting:** Notei que a IA precisa que a solicitação separe matematicamente o custo da empresa do custo do serviço.

### ✅ Tentativa 3 (Prompt Estratégico - "Nota 10")
* **Prompt:** *"Atue como um consultor financeiro para empresas de estética automotiva e higienização residencial. Com base nos documentos fornecidos, crie uma tabela separando: 1) Custos Fixos mensais, 2) Custos Variáveis por serviço. Em seguida, explique como aplicar combos promocionais para bancos de carro e teto."*
* **Resultado:** Excelente. A IA separou aluguel/marketing (fixo) de produtos químicos/deslocamento (variável) e sugeriu a técnica de ancoragem: cobrar R$150 nos bancos e oferecer o teto (que custaria R$80) com desconto no combo.

---

## 📖 Miniguia de Estudo (Entrega Final)

### 1. Resumo Estruturado: O Método de Precificação
A precificação correta não é baseada em "achismo" ou apenas em dar "5% de desconto". Ela se sustenta em três pilares:
* **Mapeamento de Custos:** Saber exatamente quanto custa manter o negócio aberto (Fixo) e quanto custa o produto químico/transporte para cada casa de cliente (Variável).
* **Tempo vs. Dinheiro:** A precificação deve considerar a hora de trabalho. Um serviço de R$180 feito em 1h30 é mais lucrativo que um de R$220 que leva 3 horas.
* **Margem de Lucro Projetada:** O mercado atual permite margens na casa de 70%, desde que a percepção de valor (qualidade dos produtos, posicionamento nas redes sociais) acompanhe o preço cobrado.

### 2. Glossário do Empreendedor de Higienização
* **Custo Fixo:** Despesas que existem independentemente de você ter clientes no mês (ex: internet, marketing, celular).
* **Custo Variável:** Gastos gerados apenas quando um serviço é executado (ex: produtos químicos, combustível, pedágio).
* **Margem de Contribuição:** O quanto sobra do preço de venda após retirar os custos variáveis. É o dinheiro que vai pagar os custos fixos e gerar lucro.
* **Precificação Baseada em Valor:** Cobrar pela transformação e qualidade percebida pelo cliente, e não apenas pelo preço dos produtos utilizados.
* **Ticket Médio:** O valor médio que cada cliente gasta com você. Aumenta-se o ticket oferecendo *combos* (ex: Sofá + Impermeabilização ou Bancos + Teto automotivo).

### 3. 🤖 Prompts Reutilizáveis
Deixe estes prompts salvos para usar no NotebookLM ou ChatGPT sempre que precisar atualizar seus preços:

> **Para análise de um novo serviço:** > *"Vou começar a oferecer limpeza de [TIPO DE ESTOFADO/MÓVEL]. Meu custo estimado com produtos é de R$ [X] e levarei cerca de [Y] horas. Considerando que minha hora técnica custa R$ [Z], me ajude a formular 3 opções de preços para apresentar ao cliente: um pacote Básico, um Intermediário e um Premium."*

> **Para cálculo de Combos:** > *"Baseado nas fontes anexadas sobre 'como fazer orçamento', quero oferecer um combo de limpeza de sofá + higienização de colchão. O sofá custaria R$ [X] e o colchão R$ [Y]. Crie um roteiro de vendas persuasivo oferecendo esses dois serviços juntos com uma ancoragem de preço atrativa."*

> **Para análise de custos:** > *"Revise minha lista de custos a seguir e classifique-os em Fixos e Variáveis. Depois, me diga se estou esquecendo de algum custo oculto comum em negócios de higienização de estofados: [INSERIR LISTA DE GASTOS]."*

---
*Projeto desenvolvido para aprimoramento de estudos em Inteligência Artificial e gestão de negócios.*
