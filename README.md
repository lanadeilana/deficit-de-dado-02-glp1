
## 🇧🇷 Português

# Déficit de Dado — ed002

## A injeção que virou desejo e o mercado que entrou em colapso

Notebooks e visualizações da segunda edição da newsletter [Déficit de Dado](https://lanadeilana.substack.com).

A ed001 mostrou que o mercado fitness brasileiro foi construído em cima da insatisfação com o corpo. A ed002 mostra o que acontece quando aparece uma "solução" — o mercado se adapta, incorpora, e continua lucrando do mesmo jeito.

---

## Notebooks

### `notebook_01_buscas.ipynb`

Série histórica de interesse por GLP-1 no Google Brasil entre 2019 e 2025.

* Fonte: Google Trends via `pytrends`
* Termos analisados: "ozempic", "semaglutida", "canetas emagrecedoras", "dieta para emagrecer"
* Gráficos: série histórica com marcos anotados + momento em que "canetas emagrecedoras" ultrapassou "dietas" em volume de busca

**Atenção:** a API do Google Trends bloqueia requisições em alguns ambientes. Se der erro 403, tenta rodar com VPN ou em horário de menor tráfego. O `trends_raw.csv` com os dados já coletados está incluído no repositório.

---

### `notebook_02_mercado.ipynb`

Crescimento do mercado de GLP-1 no Brasil e evolução de sobrepeso e obesidade na população.

* Fontes: IBGE PNS 2013 e 2019, Vigitel/MS 2023, Atlas Mundial da Obesidade 2025, relatórios Itaú BBA e UBS
* Gráficos: evolução da obesidade no BR (2006–2025), crescimento do mercado GLP-1 em R$ bilhões com projeções até 2030, participação de GLP-1 na receita das grandes redes farmacêuticas

---

### `notebook_03_fitness.ipynb`

Crescimento do mercado fitness brasileiro no mesmo período do boom dos GLP-1.

* Fontes: EY Panorama Setorial Fitness Brasil 2024, relatórios de resultados SmartFit (RI B3)
* Gráficos: dois eixos com alunos em academia vs mercado GLP-1 na mesma linha do tempo, receita líquida SmartFit por ano, crescimento das empresas do "pacote Ozempic" na bolsa

---

## Gráficos gerados

| Arquivo                           | Notebook | Descrição                                  |
| --------------------------------- | -------- | ------------------------------------------ |
| `nb01_boom_buscas.png`            | 01       | Série histórica de buscas por GLP-1 no BR  |
| `nb01_canetas_vs_dieta.png`       | 01       | Canetas emagrecedoras vs dietas em 2025    |
| `nb02_obesidade_br.png`           | 02       | Evolução de obesidade e sobrepeso no BR    |
| `nb02_mercado_glp1.png`           | 02       | Mercado GLP-1 em R$ bi (2019–2030)         |
| `nb02_market_share_farmacias.png` | 02       | GLP-1 como % da receita das farmácias      |
| `nb03_fitness_vs_glp1.png`        | 03       | Academia vs GLP-1 — dois eixos             |
| `nb03_smartfit_receita.png`       | 03       | Receita líquida SmartFit por ano           |
| `nb03_pacote_ozempic.png`         | 03       | Crescimento das empresas do pacote Ozempic |

---

## Como rodar

```bash
conda activate midia
pip install pytrends
jupyter notebook
```

Ambiente testado: Python 3.10, conda, Windows 10.

---

## Fontes de dados

| Dado                     | Fonte                                    | Acesso               |
| ------------------------ | ---------------------------------------- | -------------------- |
| Interesse de busca       | Google Trends (pytrends)                 | API pública          |
| Sobrepeso e obesidade BR | IBGE PNS 2013 e 2019                     | ibge.gov.br          |
| Obesidade BR 2023        | Vigitel — Ministério da Saúde            | saude.gov.br         |
| Obesidade global 2025    | Atlas Mundial da Obesidade (WOF)         | worldobesity.org     |
| Mercado GLP-1 BR         | Itaú BBA, UBS, BTG Pactual               | citados em imprensa  |
| Mercado fitness BR       | EY Panorama Setorial Fitness Brasil 2024 | ey.com/br            |
| Dados SmartFit           | RI SmartFit (SMFT3)                      | ri.smartfit.com.br   |
| Track&Field resultados   | RI Track&Field (TFCO3)                   | ri.tracefield.com.br |

---

## Newsletter

[lanadeilana.substack.com](https://lanadeilana.substack.com)

Publicação quinzenal. Análise de dados sobre corpo, comportamento e fit culture no Brasil.

← [ed001 — Treinar pra poder comer](https://github.com/lanadeilana/deficit-de-dado-01-Treinar-pra-poder-comer)

---

## 🇺🇸 English

# Data Deficit — ed002

## The injection that became desire and the market that bent instead of breaking

Notebooks and visualizations from the second edition of the [Data Deficit](https://lanadeilana.substack.com) newsletter.

Edition 001 showed how the Brazilian fitness market was built on body dissatisfaction. Edition 002 explores what happens when a “solution” appears — the market adapts, absorbs it, and keeps profiting anyway.

---

## Notebooks

### `notebook_01_buscas.ipynb`

Historical time series of interest in GLP-1 on Google Brazil from 2019 to 2025.

* Source: Google Trends via `pytrends`
* Terms analyzed: "ozempic", "semaglutide", "weight loss pens", "weight loss diet"
* Charts: annotated time series + the moment when "weight loss pens" surpassed "diet" in search volume

**Note:** The Google Trends API may block requests in some environments. If you get a 403 error, try running with a VPN or during off-peak hours. The `trends_raw.csv` file with pre-collected data is included in the repository.

---

### `notebook_02_mercado.ipynb`

Growth of the GLP-1 market in Brazil and trends in overweight and obesity.

* Sources: IBGE PNS 2013 and 2019, Vigitel/MS 2023, World Obesity Atlas 2025, Itaú BBA and UBS reports
* Charts: obesity trends in Brazil (2006–2025), GLP-1 market growth in BRL billions with projections through 2030, GLP-1 share in major pharmacy chains’ revenue

---

### `notebook_03_fitness.ipynb`

Growth of the Brazilian fitness market during the same period as the GLP-1 boom.

* Sources: EY Fitness Sector Overview Brazil 2024, SmartFit earnings reports (B3 IR)
* Charts: dual-axis view of gym memberships vs GLP-1 market over time, SmartFit annual net revenue, growth of “Ozempic basket” companies in the stock market

---

## Generated charts

| File                              | Notebook | Description                              |
| --------------------------------- | -------- | ---------------------------------------- |
| `nb01_boom_buscas.png`            | 01       | GLP-1 search trend in Brazil             |
| `nb01_canetas_vs_dieta.png`       | 01       | Weight loss pens vs diets in 2025        |
| `nb02_obesidade_br.png`           | 02       | Overweight and obesity trends in Brazil  |
| `nb02_mercado_glp1.png`           | 02       | GLP-1 market in BRL billions (2019–2030) |
| `nb02_market_share_farmacias.png` | 02       | GLP-1 as % of pharmacy revenue           |
| `nb03_fitness_vs_glp1.png`        | 03       | Gym vs GLP-1 — dual axis                 |
| `nb03_smartfit_receita.png`       | 03       | SmartFit annual net revenue              |
| `nb03_pacote_ozempic.png`         | 03       | Growth of the Ozempic basket companies   |

---

## How to run

```bash
conda activate midia
pip install pytrends
jupyter notebook
```

Tested environment: Python 3.10, conda, Windows 10.

---

## Data sources

| Data                            | Source                                 | Access               |
| ------------------------------- | -------------------------------------- | -------------------- |
| Search interest                 | Google Trends (pytrends)               | Public API           |
| Overweight and obesity (Brazil) | IBGE PNS 2013 and 2019                 | ibge.gov.br          |
| Obesity in Brazil (2023)        | Vigitel — Ministry of Health           | saude.gov.br         |
| Global obesity (2025)           | World Obesity Atlas (WOF)              | worldobesity.org     |
| GLP-1 market (Brazil)           | Itaú BBA, UBS, BTG Pactual             | cited in media       |
| Fitness market (Brazil)         | EY Fitness Sector Overview Brazil 2024 | ey.com/br            |
| SmartFit data                   | SmartFit IR (SMFT3)                    | ri.smartfit.com.br   |
| Track&Field results             | Track&Field IR (TFCO3)                 | ri.tracefield.com.br |

---

## Newsletter

[lanadeilana.substack.com](https://lanadeilana.substack.com)

Biweekly publication. Data analysis on body, behavior, and fitness culture in Brazil.

← [ed001 — Training so you can eat](https://github.com/lanadeilana/deficit-de-dado-01-Treinar-pra-poder-comer)
