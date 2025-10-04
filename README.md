# Freeze Monster e Space Invaders

## Visão Geral

Este projeto contém dois jogos baseados em Java: Freeze Monster e Space Invaders. Cada jogo possui sua própria lógica e utiliza o padrão de design Factory Method para criar instâncias de objetos do jogo. Ambos foram desenvolvidos para a conclusão da disciplina de Princípios e Padrões de Projeto na Faculdade de Computação.

## Estrutura do Projeto

- **`BadnessBoxSprite.java`**: Contêiner para objetos `BadSprite`, permitindo agrupar vários sprites ruins.
- **`BadSprite.java`**: Classe abstrata representando um sprite ruim genérico com comportamentos e propriedades básicas.
- **`FreezeBeam.java`**: Implementa um tipo específico de `BadSprite` que representa um raio congelante.
- **`Slime.java`**: Implementa um tipo específico de `BadSprite` que representa gosma.
- **`Woody.java`**: Estende a classe `Player` para representar o personagem jogador Woody.
- **`FreezeMonsterBoard.java`**: Gerencia a lógica do jogo "Freeze Monster".
- **`Bomb.java`**: Implementa um tipo específico de `BadSprite` que representa uma bomba.
- **`BomberSprite.java`**: Estende `BadnessBoxSprite` para representar um sprite bombardeiro.
- **`Shot.java`**: Implementa um tipo específico de `BadSprite` que representa um tiro disparado pelo jogador.
- **`SpaceInvadersBoard.java`**: Gerencia a lógica do jogo "Space Invaders".
- **`Player.java`**: Representa um personagem jogador genérico.
- **`MainFrame.java`**: Configura a janela principal do jogo.
- **`Sprite.java`**: Classe base para todos os sprites.
- **`Commons.java`**: Interface que define constantes usadas em todo o projeto.
- **`FreezeMonsterGame.java`**: Classe principal que inicializa o jogo "Freeze Monster".
- **`SpaceInvadersGame.java`**: Classe principal que inicializa o jogo "Space Invaders".
- **`AbstractBoard.java`**: Classe abstrata que define a estrutura básica de um tabuleiro de jogo.

## Padrão Factory Method

O padrão Factory Method é utilizado para criar instâncias de objetos do jogo sem especificar a classe exata do objeto a ser criado, promovendo flexibilidade e reutilização do código.

### Classes Principais

- **`AbstractBoard`**: Define métodos abstratos `createPlayers` e `createPlayer`.
- **`FreezeMonsterBoard`**: Implementa `createPlayer` para criar uma instância de `Woody`.
- **`MainFrame`**: Define o método abstrato `createBoard`.
- **`FreezeMonsterGame`**: Implementa `createBoard` para criar uma instância de `FreezeMonsterBoard`.
- **`SpaceInvadersGame`**: Implementa `createBoard` para criar uma instância de `SpaceInvadersBoard`.

## Jogos

### Freeze Monster

No jogo Freeze Monster, o jogador controla o personagem Woody para navegar pelo tabuleiro, evitando ou interagindo com vários sprites como raios congelantes, gosmas e bombas.

#### Como Executar

1. Clone o repositório para sua máquina local.
2. Abra o projeto no IntelliJ IDEA.
3. Certifique-se de que todas as dependências estão resolvidas.
4. Execute a classe `FreezeMonsterGame` para iniciar o jogo Freeze Monster.

#### Controles

- **Setas do Teclado**: Movem Woody para cima, baixo, esquerda ou direita.

### Space Invaders

No jogo Space Invaders, o jogador controla um canhão para atirar em invasores espaciais que descem pelo tabuleiro.

#### Como Executar

1. Clone o repositório para sua máquina local.
2. Abra o projeto no IntelliJ IDEA.
3. Certifique-se de que todas as dependências estão resolvidas.
4. Execute a classe `SpaceInvadersGame` para iniciar o jogo Space Invaders.

#### Controles

- **Setas do Teclado**: Movem o canhão para a esquerda ou direita.
- **Barra de Espaço**: Dispara tiros.

## Licença

Este projeto está licenciado sob a Licença MIT. Veja o arquivo `LICENSE` para mais detalhes.
