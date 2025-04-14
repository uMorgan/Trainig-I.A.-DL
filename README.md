🧠🎮 Análise Comparativa do Desempenho dos Algoritmos DQN e PPO em Aprendizagem por Reforço Profundo Aplicada a Jogos Digitais
📘 Descrição do Projeto
Este projeto tem como objetivo comparar o desempenho de dois algoritmos de Aprendizagem por Reforço Profundo (Deep Reinforcement Learning - DRL): Deep Q-Network (DQN) e Proximal Policy Optimization (PPO). A análise é feita em um ambiente de jogo digital, com foco em aspectos como eficiência de aprendizado, estabilidade, recompensa média e tempo de treinamento.

A iniciativa busca compreender melhor as vantagens e desvantagens de cada abordagem (baseada em valor vs. baseada em política), além de identificar cenários onde um algoritmo se sobressai ao outro.

🧑‍💻 Autores
Ana Luisa da Silva Lima

João Morgan de Almeida Lins do Vale

E-mail: j.vale@cs.unipe.edu.br

Telefone: (83) 99123-4432

Lucas Araujo Costa

E-mail: lcosta@cs.unipe.edu.br

Telefone: (83) 98657-0820

Prof. Dr. Jose Raul de Brito Andrade (Orientador)

E-mail: jrandrade@unipe.edu.br

Telefone: (83) 99604-5325

🎯 Objetivos
Objetivo Geral
Comparar o desempenho dos algoritmos DQN e PPO em tarefas de DRL aplicadas a jogos digitais.

Objetivos Específicos
Realizar uma revisão bibliográfica sobre DQN e PPO.

Implementar e treinar ambos os algoritmos em um ambiente de jogo.

Avaliar os modelos com base em métricas quantitativas.

Analisar os resultados e discutir os pontos fortes e fracos de cada abordagem.

🛠️ Tecnologias Utilizadas
Python 3.11+

Stable Baselines3 (SB3)

Gymnasium

Matplotlib / Seaborn (visualização)

Pandas / NumPy (análise de dados)

🎮 Ambiente de Teste
O ambiente de jogo utilizado foi o Breakout (versão Atari), acessado via Gymnasium. Esse jogo é comumente usado em benchmarks de DRL por sua complexidade moderada e representação visual clara, facilitando a avaliação dos algoritmos.

🧪 Metodologia
Revisão da Literatura: Estudo teórico dos fundamentos de DRL e dos algoritmos DQN e PPO.

Implementação: Uso da biblioteca Stable Baselines3 para treinar os modelos.

Treinamento: Cada agente foi treinado por 20 milhões de frames em condições equivalentes.

Coleta de Dados: Métricas registradas durante o treinamento, como recompensa média e estabilidade.

Análise dos Resultados: Geração de gráficos e discussão sobre desempenho, eficiência e robustez dos algoritmos.

📊 Métricas Avaliadas
Recompensa Média por Episódio

Número de Episódios até a Convergência

Estabilidade do Desempenho

Retorno Acumulado

Tempo de Treinamento

📁 Organização do Projeto
bash
Copiar
Editar
📦 drl-comparativo
├── 📂 data/                 # Dados coletados durante os treinos
├── 📂 models/               # Modelos treinados (.zip ou .pt)
├── 📂 notebooks/            # Jupyter Notebooks de análise e visualização
├── 📂 src/                  # Scripts de treinamento
│   ├── train_dqn.py
│   └── train_ppo.py
├── README.md               # Este arquivo
└── requirements.txt        # Dependências do projeto
📈 Resultados Esperados
Espera-se identificar diferenças claras entre os algoritmos DQN e PPO em termos de:

Velocidade de aprendizado

Estabilidade durante o treino

Recompensas alcançadas

Robustez ao longo do tempo

Com isso, este estudo contribui para orientar futuras escolhas de algoritmos de DRL em ambientes digitais e aplicações práticas de IA.

📚 Referências Principais
Mnih et al. (2015) – Human-level control through deep reinforcement learning

Schulman et al. (2017) – Proximal Policy Optimization Algorithms

De La Fuente & Vidal (2024) – A Comparative Study of Deep Reinforcement Learning Models: DQN vs PPO vs A2C

Lista completa de referências disponível no artigo/documento principal.
