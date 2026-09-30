[readme_md.md](https://github.com/user-attachments/files/32880061/readme_md.md)
# Inteligência de Dados Aplicada a Compras Governamentais
> **Aplicação do Princípio de Pareto nos Dados da API do PNCP (Lei nº 14.133/2021)**

![Python](https://img.shields.io/badge/Python-3.8+-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?style=for-the-badge&logo=python&logoColor=white)
![Status](https://img.shields.io/badge/Status-Concluído-brightgreen?style=for-the-badge)

## 📌 Sobre o Projeto

Este projeto analisa a concentração financeira e volumétrica das contratações públicas no Brasil com base nos dados abertos do **Portal Nacional de Contratações Públicas (PNCP)** sob a vigência da **Nova Lei de Licitações (Lei nº 14.133/2021)**.

Utilizando a linguagem Python e bibliotecas de análise de dados, extraímos e processamos registros via API oficial para aplicar o **Princípio de Pareto (Regra 80/20)**. O objetivo é evidenciar a concentração dos gastos governamentais e demonstrar como a inteligência de dados pode otimizar estratégias de auditoria, *compliance* e fiscalização de órgãos de controle como TCU e CGU.

---

## 📊 Principais Resultados

* **Volume Processado:** 3.936 contratos homologados distribuídos em 846 órgãos públicos.
* **Montante Analisado:** Mais de **R$ 6,1 bilhões** em contratações públicas.
* **Curva de Pareto:** Demonstrou estatisticamente que a maioria dos recursos públicos executados está concentrada em uma minoria de instituições.
* **Divergência Volumétrica vs. Financeira:** Os órgãos com maior quantidade de contratos (como comandos militares e órgãos estaduais de saúde) não são necessariamente os mesmos que concentram os maiores volumes orçamentários (como instituições federais de ensino e administrações de grande porte).

---

## 🛠️ Tecnologias e Ferramentas Utilizadas

* **Linguagem:** [Python](https://www.python.org/)
* **Requisições HTTP:** `requests` (Integração com endpoints Swagger da API de Dados Abertos do Compras.gov.br)
* **Tratamento e Manipulação de Dados:** `pandas`
* **Visualização de Dados:** `matplotlib`

---

## ⚙️️ Funcionalidades do Código

1. **Extração de Dados:** Consumo automatizado dos *endpoints* oficiais da API de Dados Abertos do PNCP.
2. **Limpeza e Tratamento:** Tratamento de valores nulos, conversão de tipos de dados e padronização das informações dos contratos.
3. **Agregação e Métricas:** Agrupamento por órgãos contratantes, cálculo de volume financeiro total homologado e contagem de contratos.
4. **Análise de Pareto:** Cálculo percentual acumulado para geração da Curva de Pareto (Top 20 órgãos).
5. **Visualizações Gráficas:**
   * Top 10 órgãos por quantidade de contratos.
   * Top 10 órgãos por valor total homologado (R$).
   * Curva de Pareto da concentração de valores.
   * Distribuição espacial dos gastos públicos por estado (Mapa Coroplético).

---

## 🚀 Como Executar o Projeto

### Pré-requisitos

Certifique-se de ter o Python 3.8+ instalado em sua máquina.

### Passos para execução

1. **Clone o repositório:**
   ```bash
   git clone https://github.com/seu-usuario/nome-do-repositorio.git
   cd nome-do-repositorio
   ```

2. **Crie um ambiente virtual (opcional, mas recomendado):**
   ```bash
   python -m venv venv
   # No Linux/macOS:
   source venv/bin/activate
   # No Windows:
   .\venv\Scripts\activate
   ```

3. **Instale as dependências:**
   ```bash
   pip install requests pandas matplotlib
   ```

4. **Execute o script principal:**
   ```bash
   python main.py
   ```

---

## 👥 Autores

* **Kauã Fernando Lamas Pereira** - *Estudante de Inteligência em Análise de Dados* - Faculdade SENAI Suíço-Brasileira
* **Cauan Teixeira dos Santos** - *Estudante de Inteligência em Análise de Dados* - Faculdade SENAI Suíço-Brasileira

---

## 🙏 Agradecimentos

Agradecemos à **Faculdade de Tecnologia SENAI Suíço-Brasileira** pelo suporte institucional e infraestrutura disponibilizada, e aos professores **Rafael Orsi** e **Felipe Camargo** pelas orientações e revisão crítica que contribuíram significativamente para este trabalho.

---

## 📜 Referências

* BRASIL. **Lei nº 14.133, de 1º de abril de 2021**. Lei de Licitações e Contratos Administrativos. Brasília, DF, 2021.
* BRASIL. Ministério da Gestão e da Inovação em Serviços Públicos. **API de Dados Abertos do Compras.gov.br e PNCP**. Brasília, 2025.
* JURAN, Joseph M. **Juran na Liderança pela Qualidade: Um Guia para Executivos**. São Paulo: Pioneira, 1990.
* MCKINNEY, Wes. **Python para Análise de Dados**: Tratamento de Dados com Pandas, NumPy e IPython. São Paulo: Novatec Editora, 2018.
* PARETO, Vilfredo. **Manual de Economia Política**. São Paulo: Nova Cultural, 1987.
