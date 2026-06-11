# Automação de Processos e Auditoria de Documentos com IA

![ChatGPT](https://img.shields.io/badge/ChatGPT-74AA9C?style=for-the-badge&logo=openai&logoColor=white)
![Gemini](https://img.shields.io/badge/Gemini-9B51E0?style=for-the-badge&logo=googlegemini&logoColor=white)

Este projeto apresenta um estudo de caso focado em uma solução real de negócio, desenvolvida por mim como iniciativa de um Plano de Desenvolvimento Individual (PDI) e aplicada oficialmente no ambiente corporativo da Athié Wohnrath, empresa de arquitetura e construção[cite: 1, 2]. A ferramenta automatiza as etapas de auditoria, extração de dados e separação física de documentos fiscais e financeiros (Notas Fiscais de Serviços e de Obras - SAF)[cite: 1, 2].

---

### O Desafio Inicial

No formato de trabalho anterior, a conferência das informações das Notas Fiscais era feita de forma totalmente manual usando um arquivo PDF único gerado pelo sistema[cite: 1]. Esse modelo trazia algumas dificuldades diárias:

| Ponto Crítico | Impacto no Processo |
| :--- | :--- |
| Tempo elevado | Consumia de 1 a 2 horas por dia dependendo do volume de dados[cite: 1]. |
| Erros manuais | Análises repetitivas de numerações longas aumentavam o risco de falhas por cansaço operacional[cite: 1]. |
| Limitação de sistema | O sistema principal da empresa não atendia o fluxo específico de extração e separação de PDFs exigido para os clientes VIP[cite: 1]. |

---

### A Solução Desenvolvida

Com o suporte do Google Gemini para a estruturação lógica das instruções[cite: 1], foi criado um assistente de inteligência artificial customizado (Custom GPTs) na plataforma da OpenAI[cite: 1]. A solução foi estruturada com regras e instruções detalhadas para tratar os arquivos em lotes[cite: 1]:

| Etapa | Ação Executada pela IA |
| :--- | :--- |
| Mapeamento | Identifica o começo de cada lote através das Autorizações de Pagamento[cite: 1]. |
| Extração Estruturada | Analisa o PDF original, coleta os dados principais (Número da NF, Fornecedor, CNPJ, Vencimentos e Impostos) e gera um relatório pronto em Excel (`.xlsx`)[cite: 1, 2]. |
| Separação de Arquivos | Aciona ferramentas internas de código para usar as bibliotecas de Python (`PyPDF2` ou `PyMuPDF`), recortando as páginas originais e salvando cada Nota Fiscal em um arquivo individual, mantendo as assinaturas e o layout original[cite: 1]. |

---

### Eficiência de Tempo Operacional

Gráfico comparativo do tempo gasto por lote de romaneio[cite: 1]:

* **Processo Manual Antigo (Média de 90 minutos):**
  `████████████████████████████████████████` (100%)
* **Processo Automatizado Atual (Média de 20 minutos):**
  `████████` (22%)

---

### Resultados e Ganhos Práticos

* **Ganho de tempo:** O processo que demorava de 1 a 2 horas passou a ser feito em apenas 20 minutos[cite: 1].
* **Confiabilidade:** Eliminação de erros de digitação e travas no prompt para impedir que a inteligência artificial invente dados ou impostos zerados[cite: 1].
* **Atendimento Customizado:** Permitiu realizar a separação e organização exigida pelos clientes VIP de forma automatizada, gerando eficiência direta para a operação da construtora[cite: 1].

---

### Documentação do Projeto

* [Visualizar Engenharia de Prompt e Regras de Negócio](./docs/prompt_estruturado.md)
