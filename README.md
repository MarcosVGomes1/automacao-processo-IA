# Automação de Processos e Auditoria de Documentos com IA
![ChatGPT](https://img.shields.io/badge/ChatGPT-74AA9C?style=for-the-badge&logo=openai&logoColor=white)

Este meu projeto apresenta um estudo de caso focado em uma solução real de negócio, desenvolvida por mim como iniciativa de um Plano de Desenvolvimento Individual (PDI) e aplicada oficialmente no ambiente corporativo da empresa em que eu trbalho. A ferramenta automatiza as etapas de auditoria, extração de dados e separação física de documentos fiscais e financeiros.

---

### O Desafio Inicial

No formato de trabalho anterior, a conferência das informações das Notas Fiscais era feita de forma totalmente manual usando um arquivo PDF único gerado pelo sistema, esse modelo trazia algumas dificuldades diárias:

* **Tempo elevado:** Consumia de 1 a 2 horas por dia dependendo do volume de dados.
* **Erros manuais:** Análises repetitivas de numerações longas aumentavam o risco de falhas por cansaço operacional.
* **Limitação de sistema:** O sistema principal da empresa não atendia o fluxo específico de extração e separação de PDFs exigido para os clientes VIP.

---

### A Solução Desenvolvida

Foi criado um assistente de inteligência artificial customizado (Custom GPTS) na plataforma da OpenAI. A solução foi estruturada com regras e instruções detalhadas para tratar os arquivos em lotes:

* **Mapeamento:** Identifica o começo de cada lote através das Autorizações de Pagamento.
* **Extração Estruturada:** analise o PDF original, coleta os dados principais (Número da NF, Fornecedor, CNPJ, Vencimentos e Impostos) e gera um relatório pronto em Excel (.xlsx).
* **Separação de Arquivos:** Aciona ferramentas internas de código para usar as bibliotecas de Python (PyPDF2 ou PyMuPDF), recortando as páginas originais e salvando cada Nota Fiscal em um arquivo individual, mantendo as assinaturas e o layout original.

---

### Resultados e Ganhos Práticos

* **Ganho de tempo:** O processo que demorava de 1 a 2 horas passou a ser feito em apenas 20 minutos.
* **Confiabilidade:** Eliminação de erros de digitação e travas no prompt para impedir que a inteligência artificial invente dados ou impostos zerados.
* **Atendimento Customizado:** Permitiu realizar a separação e organização exigida pelos clientes VIP de forma automatizada.

---

### Documentação do Projeto

* [Visualizar Engenharia de Prompt e Regras de Negócio](./docs/prompt_estruturado.md)
