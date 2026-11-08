# Tetris em Java

Projeto Integrador desenvolvido como trabalho acadêmico. Consiste em uma implementação do jogo Tetris em Java, com interface gráfica construída em Swing.

**Autor:** Guilherme da Luz Weber

## Descrição

O jogo apresenta um tabuleiro de 10 colunas por 22 linhas, no qual as peças (tetrominós) caem automaticamente. O jogador movimenta e gira as peças para completar linhas horizontais, que são removidas do tabuleiro. A quantidade de linhas removidas é exibida na barra de status, e a partida termina quando uma nova peça não pode mais ser posicionada.

## Estrutura do repositório

```
src/main/java/tetris/Tetris.java   Classe principal; cria a janela e inicia o jogo
src/main/java/tetris/Board.java    Tabuleiro, lógica do jogo e controle do teclado
src/main/java/tetris/Shape.java    Definição e rotação das peças
.project, .classpath               Configuração do projeto no Eclipse
```

## Requisitos

- Java Development Kit (JDK) 7 ou superior

## Execução

Pelo terminal, a partir da raiz do repositório:

```
javac -d bin src/main/java/tetris/*.java
java -cp bin tetris.Tetris
```

Pelo Eclipse: **File > Import > Existing Projects into Workspace**, selecionar a pasta do repositório e executar a classe `Tetris`.

## Controles

| Tecla            | Ação                          |
|------------------|-------------------------------|
| Seta esquerda    | Move a peça para a esquerda   |
| Seta direita     | Move a peça para a direita    |
| Seta para baixo  | Gira a peça para a direita    |
| Seta para cima   | Gira a peça para a esquerda   |
| Espaço           | Derruba a peça imediatamente  |
| D                | Desce a peça uma linha        |
| P                | Pausa e retoma o jogo         |

## Tecnologias

- Java
- Swing e AWT (interface gráfica e eventos de teclado)
