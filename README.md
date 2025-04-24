
---

## 🏡 Sistema de Recomendação de Imóveis com Agentes Inteligentes

Este projeto apresenta um sistema automatizado para recomendação de imóveis utilizando inteligência artificial e agentes colaborativos. A solução foi construída com base na biblioteca **CrewAI**, integrando modelos da OpenAI, ferramentas de busca e um banco de dados CSV com as opções de imóveis.

---

## 🚀 Objetivo do Projeto

Automatizar o processo de busca de imóveis com base nas preferências do cliente, oferecendo recomendações personalizadas a partir de dados estruturados em um arquivo CSV. O sistema utiliza agentes inteligentes com funções específicas para simular um corretor virtual.

---

## 🛠️ Tecnologias Utilizadas

- Python 3.11+
- [CrewAI](https://github.com/joaomdmoura/crewAI)
- LangChain e LangChain Tools
- OpenAI GPT-3.5 Turbo
- DuckDuckGoSearchResults (LangChain Tool)
- dotenv
- Pandas (implícito pelo CSVSearchTool)

---

## 📁 Estrutura do Projeto

```bash
.
├── recomendacao_imoveis.ipynb
├── files/
│   └── imoveis.csv
└── .env
```

---

## 🔍 Etapas do Projeto

### 1. **Importação das Bibliotecas**
Carregamento das bibliotecas e ferramentas da CrewAI, LangChain, OpenAI, busca e variáveis de ambiente.

### 2. **Configuração do Modelo LLM**
Configura e autentica o modelo `gpt-3.5-turbo-0125` da OpenAI, utilizado como motor de raciocínio dos agentes.

### 3. **Carregamento da Base de Dados**
Um arquivo CSV com dados de imóveis é carregado usando a ferramenta `CSVSearchTool`.

### 4. **Criação dos Agentes Inteligentes**
Diversos agentes com papéis específicos são criados para atuarem em conjunto.

### 5. **Definição das Tarefas**
Cada agente recebe uma tarefa correspondente ao seu papel, desde busca de imóveis até análise de mercado.

### 6. **Execução da Crew**
Os agentes trabalham de forma coordenada, com processos sequenciais, para produzir uma recomendação final.

---

## 🧠 Agentes Inteligentes

### 1. **🏘️ Corretor de Imóveis**
- **Função:** Interage com o cliente e busca imóveis compatíveis no banco de dados.
- **Objetivo:** Identificar imóveis ideais com base nas preferências fornecidas.
- **Ferramenta:** Acesso direto ao `imoveis.csv` via `CSVSearchTool`.
- **Backstory:** Especialista em imóveis, atua como consultor virtual do cliente.

---

### 2. **📈 Analista de Mercado Imobiliário**
- **Função:** Analisa tendências de valorização e depreciação de imóveis por cidade.
- **Objetivo:** Antecipar oportunidades ou riscos financeiros com base em dados históricos.
- **Backstory:** Atuário e economista imobiliário, entrega projeções embasadas.

---

### 3. **📰 Analista de Notícias Imobiliárias**
- **Função:** Agrega e interpreta notícias relevantes sobre o mercado imobiliário.
- **Objetivo:** Avaliar impacto de eventos macroeconômicos sobre os preços.
- **Backstory:** Jornalista econômico com foco em política urbana e infraestrutura.

---

### 4. **💰 Consultor Financeiro**
- **Função:** Analisa possibilidades de financiamento com base no perfil do cliente.
- **Objetivo:** Sugerir soluções financeiras viáveis para aquisição dos imóveis.
- **Backstory:** Especialista em crédito imobiliário, conhece os melhores bancos e taxas.

---

### 5. **📝 Redator de Relatórios Imobiliários**
- **Função:** Redige o relatório final para o cliente, unindo análises e imóveis recomendados.
- **Objetivo:** Apresentar dados complexos de forma clara, visual e convincente.
- **Backstory:** Profissional de comunicação com experiência em relatórios executivos.

---

## ✅ Resultados

O sistema gera uma recomendação de imóveis personalizada e justificada com base em dados históricos, notícias do setor e condições de financiamento. Ideal para clientes que desejam segurança e praticidade na busca por um novo imóvel.

---

## 💡 Potenciais Melhorias

- Interface web com Streamlit ou Flask
- Integração com banco de dados relacional
- Suporte para múltiplos perfis de cliente
- Integração com geolocalização via APIs

---
