# TEKNIKAO Hackathon - Análise de Vibrações e Manutenção Preditiva

Projeto desenvolvido no **Desafio TEKNIKAO 1 - Análise de Vibrações e Manutenção Preditiva (Indústria 4.0)**.

O desafio começou no dia **23** e terminou com a apresentação final no dia **26**, totalizando **3 dias de desenvolvimento**.

## Dados

A TEKNIKAO disponibilizou cerca de **2 GB de dados históricos de vibração**, com mais de **1 milhão de arquivos** distribuídos em diferentes pastas e configurações.

Nós coletamos esses arquivos e usamos o arquivo [`pegar_dados.py`](pegar_dados.py) para processar e consolidar tudo em um **banco de dados único**.

O banco foi mantido no repositório para facilitar o acesso da equipe, evitar que todos precisassem coletar os mesmos dados e porque o conjunto utilizado não apresentava restrições de sigilo ou conteúdo sensível.

## Propostas de valor

Durante o hackathon, a equipe desenvolveu uma interface para apoiar a análise dos dados e a manutenção preditiva.

As principais entregas foram:

- **Visão geral dos ativos**, com filtros por status, busca por máquina e leitura rápida da tendência de vibração.
- **Gráficos de evolução e projeção P-F**, com linhas de aviso, limite crítico e previsão de manutenção.
- **Kanban de manutenção**, para organizar os itens por etapa do processo, como cotação, compra, aguardando troca e manutenção concluída.
- **Relatório técnico**, com resumo dos ativos, níveis de risco e geração de PDF.

## Análises
Neste projeto, a análise foi feita a partir do banco de dados criado neste repositório, que consolida as medições históricas de vibração dos motores. A partir dele, o notebook organiza os dados, trata inconsistências, remove outliers, suaviza as séries e ajusta uma curva exponencial para estimar a evolução do RMS ao longo do tempo. Com isso, foi possível identificar possíveis cortes por manutenção, prever a aproximação aos limites de aviso e criticidade e gerar uma visão consolidada com tabelas e gráficos para apoiar decisões de manutenção e compra de peças.

https://colab.research.google.com/drive/1TcYOb_t6Al_EXMnFitQdCE_jLv9bqLGt?usp=sharing


## Resultado

A equipe ficou em **2º lugar** no hackathon.
