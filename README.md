# NoMAD Portfolio Optimization

**No MAD aproach for portfolio detection based on the [MAD Portfolio Optimization](https://mo-book.ampl.com/notebooks/02/mad-portfolio-optimization.html) experiment**

![UFABC Logo](assets/logotipo-ufabc-extenso.png)

Universidade Federal do ABC - Bacharelado em Ciência e Tecnologia Algoritmos e Estruturas de Dados 2023/Q3

Lenin Cristi

lenin.cristi@aluno.ufabc.edu.br

## Resumo do experimento

**Resumo.** Parte da escolha de um conjunto arbitrário de ações da bolsa brasileira (IBOVESPA, B3) para comparação de dois métodos de otimização de risco distintos

**Abstract.** It starts from choosing an arbitrary set of shares on the Brazilian stock exchange (IBOVESPA, B3) to compare two different risk optimization methods

## Objetivos

* A familiarização com modelos de otimização linear para a construção de portfolios de ativos financeiros que ofereçam,
ao mesmotempo, "bons" retornos ao capital inicial investido e uma "certa" proteção ao risco inerente envolvido em tais operações

* A familiarização com a linguagem de modelagem AMPL e sua utilização via Python ~no ambiente Colab da Google~** num ambiente conda reprodutível

* A experimentação / solução dos modelos com dados reais (obtidos da plataforma Yahoo Finance) via solvers de otimização linear

* Uma ligeira análise dos resultados devolvidos pelos solvers

** Foi utilizado um ambiente fora do Colab, mas sem prejuízo a reprodutibilidade ou execução no próprio Colab ou em qualquer outra nuvem de preferência

## Como analisar os resultados (sem precisar instalar ou rodar nada)

O Notebook principal está disponível com as saidas salvas [aqui](./nomad.ipynb)

## Como (gerar o ambiente para) reproduzir o experimento

### Utilizando Conda

Para criar, ativar e instalar os pacotes necessários

```bash
conda create -n ampl python=3.9
```

```bash
conda activate ampl
```

```bash
conda install amplpy numpy matplotlib scikit-learn yfinance ipykernel pandas -c defaults -c conda-forge
```

### Utilizando Conda com o arquivo environments.yml neste repositório

Para criar o ambiente com os pacotes necessários a partir de arquivo

```bash
conda env create -f environment.yml
```

### Utilizando Pip

Crie e ative um ambiente usando pip ou pyenv antes e instale os seguintes pacotes

```bash
pip install amplpy numpy matplotlib scikit-learn yfinance ipykernel pandas
```

## Como adquirir uma licença (Community Edition) do AMPL

* Visite o portal https://portal.ampl.com

* Faça o registro de usuário gratuito

* Liste suas licenças em https://portal.ampl.com/user/ampl/license/list

* Faça o download do arquivo ampl.lic gerado e o instale no local dos binários AMPL, numa instalação onde o ambiente (environment python) onde foi instalado o AMPL se chama "ampl", seria aqui:

```bash
\envs\ampl\Lib\site-packages\ampl_module_base\bin
```

Existem outros modos de ativação, como por exemplo rodar o UUID da licença com o comando "amplkey activate", mais informações [aqui](https://dev.ampl.com/ampl/free.html) e [aqui](https://dev.ampl.com/ampl/install.html)

## Referências

[1] MAD portfolio optimization<br>
https://mo-book.ampl.com/notebooks/02/mad-portfolio-optimization.html

___

CMCC - Universidade Federal do ABC (UFABC) - Santo André - SP - Brasil
