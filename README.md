# ANÁLISE COMPARATIVA DO DESEMPENHO DOS ALGORITMOS DQN E PPO EM APRENDIZAGEM POR REFORÇO PROFUNDO APLICADA A JOGOS DIGITAIS

## Autores

- **Ana Luisa da Silva Lima**  

- **João Morgan de Almeida Lins do Vale**  

- **Lucas Araujo Costa**  

- **Jose Raul de Brito Andrade (Orientador)**    

---

## Resumo

A aprendizagem por reforço profundo (Deep Reinforcement Learning – DRL) tem se destacado na resolução de problemas complexos, especialmente em jogos digitais, devido à sua capacidade de treinar agentes autônomos em ambientes dinâmicos. Este trabalho propõe uma análise comparativa do desempenho dos algoritmos Deep Q-Network (DQN) e Proximal Policy Optimization (PPO), representantes dos paradigmas de aprendizagem baseada em valor e baseada em política, respectivamente, em tarefas de DRL aplicadas a jogos digitais. A metodologia envolve a revisão da literatura, a definição de um ambiente de teste controlado, a implementação e treinamento dos modelos DQN e PPO, e a análise de métricas como recompensa média e estabilidade de aprendizado. Espera-se validar as diferenças de desempenho entre os algoritmos e identificar cenários onde cada um se destaca.

**Palavras-chave:** Aprendizagem por reforço profundo, Deep Q-Network, Proximal Policy Optimization, Jogos digitais, Inteligência artificial.

---

## Abstract

Deep Reinforcement Learning (DRL) has excelled in solving complex problems, particularly in digital games, due to its ability to train autonomous agents in dynamic environments. This work proposes a comparative analysis of the performance of the Deep Q-Network (DQN) and Proximal Policy Optimization (PPO) algorithms, representatives of value-based and policy-based learning paradigms, respectively, in DRL tasks applied to digital games. The study includes a literature review, definition of a test environment, implementation and training of models, and performance metric analysis.

**Keywords:** Deep reinforcement learning, Deep Q-Network, Proximal Policy Optimization, Digital games, Artificial intelligence.

---

## Introdução

A aprendizagem por reforço profunda (DRL) é amplamente utilizada na resolução de problemas complexos, com destaque para aplicações em jogos digitais. Os algoritmos DQN (baseado em valor) e PPO (baseado em política) foram escolhidos por representarem abordagens complementares na DRL. Comparar seus desempenhos possibilita identificar forças e limitações que guiam o desenvolvimento de aplicações mais eficazes.

O objetivo principal deste trabalho é analisar e comparar o desempenho dos algoritmos DQN e PPO em tarefas de DRL aplicadas a jogos. Para isso, foram definidos os seguintes objetivos específicos:

- Revisar a literatura sobre DRL e os algoritmos DQN e PPO;
- Definir um ambiente de teste controlado;
- Implementar e treinar os modelos;
- Coletar e analisar métricas de desempenho.

---

## Metodologia

### 1. Revisão da Literatura

A pesquisa iniciou-se com uma revisão bibliográfica sobre DRL, focando nas diferenças teóricas entre DQN (off-policy) e PPO (on-policy), guiada por fontes como Sutton & Barto (2018), Mnih et al. (2015), e Schulman et al. (2017).

### 2. Ambiente de Teste

O ambiente utilizado foi o jogo **Breakout** do Gymnasium. Este ambiente é amplamente adotado em estudos de DRL, oferecendo recompensas imediatas e um cenário ideal para avaliar estratégias distintas.

### 3. Implementação e Treinamento

Os modelos foram implementados com a biblioteca [Stable Baselines3 (SB3)](https://stable-baselines3.readthedocs.io/), utilizando arquiteturas padronizadas:

- **DQN:** arquitetura baseada em Mnih et al. (2015) com `experience replay`.
- **PPO:** implementação de Schulman et al. (2017), utilizando o objetivo clipado para estabilidade.

O treinamento foi feito por **20 milhões de frames** com GPU de 8 GB de RAM.

### 4. Métricas de Avaliação

- **Recompensa média por episódio**
- **Episódios até convergência**
- **Estabilidade do desempenho**
- **Retorno acumulado**
- **Tempo de treinamento**

---

## Fundamentação Teórica

- **Aprendizagem por Reforço (RL):** baseado em tentativa e erro em um MDP (SUTTON; BARTO, 1998).
- **Deep RL (DRL):** integração com redes neurais profundas para processar entradas visuais complexas (ARULKUMARAN et al., 2017).
- **DQN:** uso de CNNs com `experience replay` e `target networks` (MNIH et al., 2015).
- **PPO:** algoritmo baseado em política com atualizações seguras (SCHULMAN et al., 2017).

---

## Resultados e Discussão

Os resultados serão apresentados por meio de:

- Curvas de aprendizado
- Histogramas de recompensas
- Análises descritivas comparativas

O foco está na eficiência, estabilidade e tempo de convergência de cada algoritmo.

---

## Considerações Finais

Este estudo contribui para o entendimento das vantagens e limitações de DQN e PPO em DRL. Os dados obtidos possibilitam orientar futuras pesquisas na escolha de algoritmos conforme a complexidade dos ambientes e as necessidades de estabilidade ou performance.

Sugestões para trabalhos futuros incluem a análise de algoritmos como A2C, TD3 ou SAC, bem como a aplicação dos métodos em ambientes com estados contínuos ou parciais.

---

## Referências

- ARULKUMARAN, K. et al. *Deep Reinforcement Learning: A Brief Survey*. IEEE Signal Processing Magazine, 2017.
- DE LA FUENTE, N.; VIDAL, D. A. *A comparative study of deep reinforcement learning models: DQN vs PPO vs A2C*. ACM KDD 2024.
- FUJIMOTO, S. et al. *Addressing Function Approximation Error in Actor-Critic Methods*. ICML, 2018.
- HAARNOJA, T. et al. *Soft Actor-Critic*. ICML, 2019.
- LI, S. E. *Reinforcement Learning for Sequential Decision and Optimal Control*. Springer, 2023.
- MNIH, V. et al. *Human-level control through deep reinforcement learning*. Nature, 2015.
- MOUSAVI, S. S. et al. *Deep Reinforcement Learning: An Overview*. 2017.
- SCHULMAN, J. et al. *Proximal policy optimization algorithms*. arXiv:1707.06347, 2017.
- SUTTON, R. S.; BARTO, A. G. *Reinforcement Learning: An Introduction*. MIT Press, 2018.

---

> **Nota:** Este repositório contém os códigos e scripts necessários para executar os experimentos descritos no artigo. Certifique-se de instalar as dependências listadas em `requirements.txt`.
