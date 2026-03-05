# 📊 Análise de Receita dos Planos da Megaline

## 📖 Sobre o projeto

Este projeto tem como objetivo analisar o comportamento dos clientes e a geração de receita de dois planos de telefonia pré-paga da empresa **Megaline**: **Surf** e **Ultimate**.

A análise busca entender como o uso dos serviços (ligações, mensagens e internet) impacta a receita mensal dos usuários e identificar qual plano tende a gerar maior receita para a empresa.

O projeto envolve **preparação de dados, análise exploratória, agregações mensais e testes estatísticos** para apoiar a tomada de decisão baseada em dados.

---

# 🗂️ Conjunto de dados

O dataset contém informações de **500 clientes** da Megaline durante o ano de **2018**.

As tabelas utilizadas incluem:

- **users** — informações dos usuários
- **calls** — registros de chamadas
- **messages** — envio de mensagens
- **internet** — sessões de uso de internet
- **plans** — características dos planos oferecidos

---

# ⚙️ Etapas do projeto

## 1️⃣ Preparação dos dados
- Importação dos datasets
- Verificação de tipos de dados
- Tratamento de valores ausentes
- Conversão de datas
- Criação de variáveis adicionais

---

## 2️⃣ Agregação mensal de uso

Os dados foram agregados por **usuário e por mês**, permitindo calcular:

- total de chamadas
- total de minutos utilizados
- total de mensagens enviadas
- total de dados consumidos (internet)

---

## 3️⃣ Cálculo da receita

A receita mensal foi calculada considerando:

- valor da assinatura mensal do plano
- cobrança por minutos excedentes
- cobrança por mensagens excedentes
- cobrança por consumo adicional de internet

---

## 4️⃣ Análise exploratória de dados

Foram analisados:

- padrão de uso de chamadas
- comportamento de envio de mensagens
- consumo de internet
- distribuição da receita entre os planos

Foram utilizados gráficos como:

- histogramas
- gráficos de barras
- boxplots

para visualizar diferenças entre os planos.

---

## 5️⃣ Teste de hipóteses estatísticas

Foi realizado um **teste t para duas amostras independentes** para verificar se existe diferença estatisticamente significativa entre a **receita média mensal dos planos Surf e Ultimate**.

### Hipótese nula (H0)

A receita média mensal dos usuários do plano **Surf** é igual à receita média mensal dos usuários do plano **Ultimate**.

### Hipótese alternativa (H1)

A receita média mensal dos usuários do plano **Surf** é diferente da receita média mensal dos usuários do plano **Ultimate**.

---

# 📈 Principais insights

A análise mostrou que:

- O plano **Ultimate tende a gerar maior receita média por usuário**.
- O comportamento de uso entre os planos é relativamente semelhante em chamadas e mensagens.
- Usuários do plano Ultimate apresentam um consumo de internet ligeiramente maior.
- O teste estatístico confirmou que **a diferença de receita entre os planos é estatisticamente significativa**.

---

# 🛠️ Tecnologias utilizadas

- Python
- Pandas
- NumPy
- Matplotlib
- SciPy
- Jupyter Notebook

---

# ▶️ Como executar o projeto

Clone o repositório:

```bash
git clone https://github.com/seuusuario/megaline-plan-analysis.git

cd megaline-plan-analysis

pip install -r requirements.txt

jupyter notebook
```

