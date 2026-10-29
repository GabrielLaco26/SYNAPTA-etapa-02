# Desafio SYNAPTA - Etapa 02: Análise Exploratória do Mercado Imobiliário de São Paulo

Este repositório contém a resolução prática e analítica da **Etapa 02** do processo seletivo do **Edital SYNAPTA**. O estudo realiza uma análise exploratória de dados (EDA) sobre o mercado de aluguéis em São Paulo utilizando Python no Google Colab.

---

## 📌 Visão Geral do Projeto

O objetivo principal deste projeto é investigar o comportamento dos preços de locação na capital paulista a partir de características físicas dos imóveis (área útil, quantidade de quartos, vagas de garagem e tipologia) e de sua localização geográfica.

O trabalho combina código estruturado em Python (Pandas e Matplotlib) com documentação textual detalhada para garantir reprodutibilidade e rigor metodológico.

---

## 📂 Estrutura do Repositório

```text
├── SYNAPTA.ipynb       # Notebook Jupyter/Colab com o código e análises
├── requirements.txt    # Dependências do projeto para execução local
└── README.md           # Documentação e apresentação do repositório
```

*(Nota: O conjunto de dados `data.csv` não é redistribuído neste repositório em conformidade com as condições de uso da fonte original. Siga as instruções abaixo para obtê-lo).*

---

## 📥 Obtenção do Dataset

O conjunto de dados utilizado é o **Sao Paulo Housing Prices**, disponibilizado publicamente na plataforma Kaggle.

1. **Link Oficial para Download:** [Kaggle - Sao Paulo Housing Prices](https://www.kaggle.com/datasets/renatosn/sao-paulo-housing-prices)
2. **Instruções:**
   * Acesse o link acima e faça o download do arquivo em formato CSV (`data.csv`).
   * Salve ou faça o upload do arquivo `data.csv` no mesmo diretório/ambiente (Google Colab ou pasta local) onde o notebook `SYNAPTA.ipynb` será executado.

---

## 🛠️ Tecnologias e Bibliotecas Utilizadas

* **Linguagem:** Python 3
* **Ambiente de Desenvolvimento:** Google Colab
* **Manipulação e Tratamento de Dados:** `pandas`
* **Visualização de Dados:** `matplotlib.pyplot`

---

## 📊 Descrição dos Dados (Dataset)

O arquivo `data.csv` reúne dados do mercado imobiliário paulistano com as seguintes variáveis:

* `address`: Endereço do imóvel anunciado.
* `district`: Bairro ou distrito onde o imóvel está localizado.
* `area`: Área útil do imóvel em metros quadrados ($m^2$).
* `bedrooms`: Quantidade de quartos/dormitórios.
* `garage`: Quantidade de vagas de garagem.
* `rent`: Valor mensal do aluguel (R$).
* `type`: Categoria do imóvel (ex: Apartamento, Casa, Studio, Kitnet).
* `total`: Custo mensal total (incluindo aluguel, condomínio e taxas).

---

## 🔍 Principais Etapas da Análise

1. **Diagnóstico e Preparação dos Dados:**
   * Verificação de integridade da amostragem (11.657 registros).
   * Diagnóstico de valores ausentes (nulos) e consistência estrutural das colunas.
   * Aplicação de filtros de segurança para eliminação de dados fisicamente inconsistentes (ex: imóveis com área $\le 0$).

2. **Visualização Gráfica:**
   * **Gráfico 1:** Comparação do Preço Médio de Aluguel por Tipo de Imóvel.
   * **Gráfico 2:** Distribuição da Oferta de Aluguéis por Quantidade de Quartos.
   * **Gráfico 3:** Impacto das Vagas de Garagem no Valor Médio do Aluguel.

3. **Análise Crítica e Conclusões:**
   * Registro transparente das decisões metodológicas e limitações da amostragem.
   * Identificação do perfil da oferta e dos principais fatores de valorização do preço final.

---

## 🤖 Declaração do Uso de Inteligência Artificial

Em conformidade com as boas práticas de transparência e integridade acadêmica, declara-se que ferramentas de Inteligência Artificial Generativa foram utilizadas como suporte auxiliar nas seguintes etapas do desenvolvimento:

* **Planejamento Estrutural:** Apoio no delineamento dos passos metodológicos e na organização das células do notebook.
* **Aprimoramento do Código:** Otimização da qualidade do código-fonte desenvolvido pelo autor, visando melhorias no desempenho, legibilidade e padrões visuais dos gráficos gerados.
* **Documentação:** Auxílio na estruturação e redação final dos textos explicativos e deste arquivo `README.md`.

---

## 💡 Como Executar este Projeto

1. Faça o download ou clone este repositório.
2. Certifique-se de instalar as dependências necessárias utilizando o arquivo `requirements.txt`:
   ```bash
   pip install -r requirements.txt
   ```
3. Realize o download do arquivo `data.csv` conforme as instruções da seção **Obtenção do Dataset** e coloque-o na mesma pasta do projeto.
4. Abra o arquivo `SYNAPTA.ipynb` no **Google Colab** ou **Jupyter Notebook**.
5. Execute as células em ordem sequencial (`Ambiente de execução` > `Executar tudo`).

---

## 📝 Autor

* Desenvolvido como parte do Edital SYNAPTA 2026.