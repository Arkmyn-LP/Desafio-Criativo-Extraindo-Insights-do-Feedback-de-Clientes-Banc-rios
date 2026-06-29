# Desafio Criativo DIO - Extraindo Insights de Clientes Bancários

Este projeto apresenta a estruturação de um prompt de inteligência artificial voltado para a análise de dados de experiência do cliente (CX) no setor bancário, acompanhado de sua aplicação prática e resultados obtidos.

## 🤖 **1. Prompt Estruturado para IA**

Atue como um Analista de Dados sênior especializado em Experiência do Cliente (CX) no setor bancário.
Sua tarefa é analisar uma base de feedbacks de clientes sobre a experiência com o Internet Banking e Investimentos Digitais para identificar os principais gargalos na usabilidade, problemas técnicos e as maiores frustrações dos usuários.

### 🌐 **Contexto:**
A análise será enviada para a Diretoria de Produtos Digitais e para o time de Suporte Técnico de um grande banco. O objetivo é priorizar as correções do próximo trimestre (Q3), focando em reduzir o volume de chamados repetitivos no call center e melhorar a nota do aplicativo na App Store/Play Store.

### 📊 **Dados Disponíveis:**
Será fornecida uma lista contendo os seguintes campos por linha de comentário:
- ID do Cliente (Anônimo)
- Data/Hora do feedback
- Canal de Origem (App, Web, Reclame Aqui ou Ouvidoria)
- Texto do Feedback enviado pelo cliente
- Categoria sugerida pelo sistema (ex: Falha de Login, Lentidão, TED/PIX, Tela Branca)

### 📋 **Instruções de Análise:**
Classifique os feedbacks por Tema principal (ex: Bug Técnico, Falha de Comunicação, Dúvida de Navegação), Sentimento (Positivo, Neutro, Negativo) e Urgência (Baixa, Média, Alta).
Identifique os 3 padrões ou problemas mais críticos que estão gerando mais irritação nos clientes.
Aponte evidências textuais extraídas diretamente dos dados fornecidos, citando pequenos trechos dos comentários como prova.
Sugira pelo menos uma ação prática de melhoria tecnológica ou de comunicação para cada grande problema identificado.

### 📐 **Formato da Resposta:**
Resumo Executivo: Um parágrafo direto (até 4 linhas) focado no impacto do negócio.
Tabela de Classificação: Contendo as colunas: Tema | Sentimento Geral | Urgência | Trecho do Feedback (Evidência) | Ação Recomendada.
Top 3 Prioridades: Uma lista em tópicos ordenados com as três ações urgentes recomendadas para o time de tecnologia.

### ⚠️ **Restrições e Cuidados:**
Use única e exclusivamente os dados fornecidos na base fictícia.
Não invente métricas, estatísticas, volumes de reclamações ou causas que não estejam explicitamente comprovadas nos textos.
Não exponha ou tente adivinhar dados pessoais sensíveis (como CPFs, nomes, saldos ou senhas). Caso algum comentário traga esses dados, mascare-os com [DADO SENSÍVEL].
Use uma linguagem corporativa, executiva, técnica e totalmente focada em tomadas de decisão rápidas.

## 💾 **2. Base de Dados Analisada**

ID Cliente | Data/Hora | Canal | Texto do Feedback | Categoria Sugerida
001 | 15/07/2026 10:32 | App | Não consigo fazer login desde ontem, dá tela branca e fecha sozinho. Horrível! | Falha de Login
002 | 15/07/2026 11:00 | Web | Adorei o novo painel de investimentos, ficou muito mais fácil ver o rendimento do CDB. | Canais Digitais
003 | 15/07/2026 11:15 | Reclame Aqui | Tentei fazer um PIX urgente de R$ 500,00 e o saldo sumiu da conta mas o comprovante não gerou. Um absurdo, meu CPF é 123.456.789-00 resolvam logo! | TED/PIX
004 | 15/07/2026 13:00 | App | O aplicativo está muito lento hoje para carregar o extrato do cartão. | Lentidão
005 | 15/07/2026 14:22 | Ouvidoria | Demora de mais de 40 minutos para conseguir falar com um atendente no chat sobre uma dúvida de investimento. | Suporte

---

## 📝 **3. Resposta e Insights Gerados pela IA**

### 📊 **Resumo Executivo**

A análise dos cinco feedbacks identifica três focos prioritários: falhas técnicas críticas no aplicativo (login e estabilidade), problemas em transações PIX com potencial impacto financeiro e deficiências no atendimento digital. Esses pontos apresentam maior potencial de gerar insatisfação, aumento de chamados ao suporte e impacto na confiança dos clientes. Também foi identificado um feedback positivo relacionado à nova experiência de investimentos, indicando uma melhoria percebida na usabilidade dessa funcionalidade.

### 📈 **Tabela de Classificação dos Feedbacks**

```text
========================================================================================================================
TEMA                             | SENTIMENTO | URGÊNCIA | EVIDÊNCIA                 | AÇÃO RECOMENDADA
========================================================================================================================
Bug Técnico (Login/Estabilidade) | Negativo   | Alta     | "Não consigo fazer..."    | Priorizar correção da falha de login.
---------------------------------+------------+----------+---------------------------+----------------------------------
Usabilidade (Investimentos)      | Positivo   | Baixa    | "Adorei o novo painel..." | Manter padrão de design adotado.
---------------------------------+------------+----------+---------------------------+----------------------------------
Bug Técnico (PIX)                | Negativo   | Alta     | "O saldo sumiu..."        | Investigar processamento do PIX (CPF ocultado).
---------------------------------+------------+----------+---------------------------+----------------------------------
Desempenho                       | Negativo   | Média    | "Aplicativo muito lento..."| Otimizar consulta ao extrato.
---------------------------------+------------+----------+---------------------------+----------------------------------
Falha de Comunicação / Suporte   | Negativo   | Média    | "Demora de mais de 40m..."| Reduzir o tempo de espera no chat.
========================================================================================================================



## 🎯 4. Top 3 Prioridades Relatadas

1. Estabilização de Acesso: Corrigir imediatamente as falhas de login e estabilidade do aplicativo, eliminando os casos de tela branca e encerramento inesperado, por apresentarem impacto direto no acesso aos serviços.

2. Segurança Transacional: Investigar e corrigir o fluxo das transações PIX, especialmente situações em que há débito em conta sem geração de comprovante, além de aprimorar a comunicação do status da operação ao cliente.

3. Eficiência no Atendimento: Reduzir o volume de chamados ao suporte, melhorando o tempo de resposta do chat e oferecendo recursos de autoatendimento para dúvidas frequentes sobre investimentos.
