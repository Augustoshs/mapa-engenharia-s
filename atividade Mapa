#include <stdio.h>

// Funcao para ordenar o inventario com shellsort 
// oque e um shellsort: coloca os numeros em ordem mais rapido que os metodos simples ele compara numeros que estao distantes e vai diminuindo essa distancia ele organizar listas grandes de forma eficiente.

void ordenarInventario(int produtos[], int quantidade) {
    for (int intervalo = quantidade / 2; intervalo > 0; intervalo /= 2) {
        for (int i = intervalo; i < quantidade; i++) {
            int atual = produtos[i];
            int j = i;

            while (j >= intervalo && produtos[j - intervalo] > atual) {
                produtos[j] = produtos[j - intervalo];
                j -= intervalo;
            }

            produtos[j] = atual;
        }
    }
}

// Funcao para exibir os produtos
void mostrarInventario(int produtos[], int quantidade) {
    for (int i = 0; i < quantidade; i++) {
        printf("%d ", produtos[i]);
    }
    printf("\n");
}

// Funcao principal
int main() {
    int inventario[] = {45, 23, 78, 12, 56, 89, 67, 34};
    int totalProdutos = sizeof(inventario) / sizeof(inventario[0]);

    printf("Inventario antes da ordenacao:\n");
    mostrarInventario(inventario, totalProdutos);

    ordenarInventario(inventario, totalProdutos);

    printf("Inventario apos a ordenacao:\n");
    mostrarInventario(inventario, totalProdutos);

    return 0;
}
