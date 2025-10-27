# Desafio-Batalha-Naval
Desafio de programação para implementar o clássico Jogo da Batalha Naval

# 🚢 Desafio: Jogo da Batalha Naval

Bem-vindo ao Desafio de Implementação do Jogo da Batalha Naval! O objetivo é desenvolver uma versão jogável (via terminal ou com interface gráfica simples) do clássico jogo de estratégia.

## 🎯 Objetivo

Implementar as regras completas do Jogo da Batalha Naval, onde um jogador (ou a IA) tenta afundar a frota do oponente.

## ⚓ Regras e Requisitos Técnicos

O projeto deve cumprir os seguintes requisitos mínimos:

### A. O Tabuleiro
1.  **Tamanho:** O tabuleiro deve ser uma matriz quadrada de $10 \times 10$ (linhas de A a J e colunas de 1 a 10, por exemplo).
2.  **Representação:**
    * `~`: Água (Espaço vazio).
    * `N`: Navio.
    * `X`: Acertou um navio.
    * `O`: Errou o tiro (Água atingida).

### B. A Frota (Navios)
A frota deve ser composta pelos seguintes navios (você pode alterar o tamanho se quiser simplificar):

| Tipo de Navio | Tamanho (Casas) | Quantidade |
| :--- | :--- | :--- |
| Porta-Aviões | 5 | 1 |
| Encouraçado | 4 | 1 |
| Contratorpedeiro | 3 | 2 |
| Submarino | 2 | 1 |

### C. Funcionalidades Obrigatórias
1.  **Posicionamento:** O jogo deve permitir posicionar os navios de forma **aleatória** no tabuleiro. Os navios podem ser posicionados na horizontal ou na vertical. **(Requisito Básico)**
2.  **Turnos:** O jogo é de turnos. O jogador A ataca o tabuleiro B, depois o B ataca o A (no modo Player vs IA, o jogador ataca a IA e vice-versa).
3.  **Tiro:** O jogador insere uma coordenada (ex: `A5`).
    * Se for um acerto (`N`), a casa muda para `X`.
    * Se for um erro (`~`), a casa muda para `O`.
4.  **Condição de Vitória:** O primeiro jogador (ou IA) a afundar *todos* os navios do oponente vence. Um navio é afundado quando todas as suas células são atingidas (`X`).

5.  ## ⭐ Desafios Extras (Opcionais)

Para quem quiser ir além:

1.  **Player vs Player:** Implementar um modo onde dois jogadores jogam.
2.  **IA Básica:** Criar uma Inteligência Artificial simples que atira em coordenadas aleatórias que ainda não foram atacadas.
3.  **IA Inteligente:** Implementar uma IA mais esperta (ex: após acertar um navio, ela tenta atirar nas células adjacentes para afundá-lo).
4.  **Interface Gráfica:** Substituir o console por uma interface gráfica simples (usando Pygame, Tkinter, etc.).

5.  ## 🤝 Como Participar

Para participar e contribuir com a sua solução:

1.  **Fork** este repositório para a sua conta do GitHub.
2.  **Clone** o seu *fork* para a sua máquina local.
3.  Implemente a sua solução (a versão básica é o mínimo).
4.  Crie um **Pull Request (PR)** para este repositório com a sua solução.
    * No título do PR, inclua a linguagem utilizada (ex: `[Python] Implementação Básica do Jogo`).
    * Descreva no PR quais Desafios Extras você conseguiu implementar.
  
## 💾 Dados de Exemplo para Teste

Para facilitar a implementação e os testes, forneço dois arquivos de dados:

1.  **`TABULEIRO_VAZIO.txt`**: Estrutura de um tabuleiro $10 \times 10$ vazio.
2.  **`FROTA_EXEMPLO.txt`**: Um arquivo com o posicionamento de uma frota completa. Ele pode ser usado para carregar o tabuleiro do oponente e testar a lógica de tiro (`Acerto`, `Erro`, `Afundou`).

Sinta-se à vontade para usar, adaptar ou ignorar esses arquivos conforme a necessidade do seu projeto!

