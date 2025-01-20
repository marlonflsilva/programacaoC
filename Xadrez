#include <stdio.h>

#define MOVIMENTO_BISPO 5       // Quantidade de casas que o Bispo pode mover
#define MOVIMENTO_TORRE 5       // Quantidade de casas que a Torre pode mover
#define MOVIMENTO_RAINHA 8      // Quantidade de casas que a Rainha pode mover
#define MOVIMENTO_CAVALO_HORIZONTAL 2  // Movimento horizontal do Cavalo
#define MOVIMENTO_CAVALO_VERTICAL 1    // Movimento vertical do Cavalo

// Função recursiva para mover o Bispo
void moverBispo(int movimentoAtual) {
    if (movimentoAtual <= MOVIMENTO_BISPO) {
        printf("Bispo moveu %d casas na diagonal superior direita\n", movimentoAtual);
        moverBispo(movimentoAtual + 1);  // Chamada recursiva para mover mais uma casa
    }
}

// Função para simular a movimentação da Torre para a direita
void moverTorre() {
    for (int i = 1; i <= MOVIMENTO_TORRE; i++) {
        printf("Torre moveu %d casas para a direita\n", i);
    }
}

// Função para simular a movimentação da Rainha para a esquerda
void moverRainha() {
    for (int i = 1; i <= MOVIMENTO_RAINHA; i++) {
        printf("Rainha moveu %d casas para a esquerda\n", i);
    }
}

// Função para simular a movimentação do Cavalo (movimento em L) com loops aninhados
void moverCavalo() {
    // Loop externo (movimento vertical)
    for (int i = 1; i <= MOVIMENTO_CAVALO_VERTICAL; i++) {
        // Loop interno (movimento horizontal) com while
        int j = 1;
        while (j <= MOVIMENTO_CAVALO_HORIZONTAL) {
            if (i == 1 && j == 1) {
                continue;  // Pule o primeiro movimento, como exemplo de uso do continue
            }

            printf("Cavalo se moveu %d casas para baixo e %d casas para a esquerda\n", i, j);

            // Exemplo de uso de break: pare no movimento 2x2
            if (i == 2 && j == 2) {
                break;  // Interrompe o loop quando atingir o movimento 2x2
            }
            j++;  // Incrementa o movimento horizontal
        }
    }
}

int main() {
    printf("Movimentação do Bispo (Recursiva):\n");
    moverBispo(1);  // Começa o movimento do Bispo

    printf("\nMovimentação da Torre (Direita):\n");
    moverTorre();  // Simula a movimentação da Torre

    printf("\nMovimentação da Rainha (Esquerda):\n");
    moverRainha();  // Simula a movimentação da Rainha

    printf("\nMovimentação do Cavalo (Em L):\n");
    moverCavalo();  // Simula a movimentação do Cavalo

    return 0;
}
