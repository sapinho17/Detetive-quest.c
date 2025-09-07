#include <stdio.h>

int main() {
    int escolha;

    printf("=== DETETIVE QUEST ===\n");
    printf("Você é um detetive chamado para investigar um crime misterioso.\n");
    printf("Um homem foi encontrado morto em sua casa. Há três suspeitos.\n");
    printf("Sua missão é descobrir quem é o culpado!\n\n");

    printf("Você começa a investigação.\n");
    printf("1 - Interrogar a esposa\n");
    printf("2 - Interrogar o vizinho\n");
    printf("3 - Investigar a cena do crime\n");
    printf("Escolha: ");
    scanf("%d", &escolha);

    if (escolha == 1) {
        printf("\nA esposa parece nervosa, mas afirma que estava no mercado.\n");
        printf("Você descobre que não há testemunhas confirmando o álibi.\n");
        printf("Ela pode estar escondendo algo...\n");
    } 
    else if (escolha == 2) {
        printf("\nO vizinho diz que viu alguém entrando na casa à noite.\n");
        printf("Ele afirma que a pessoa tinha um casaco vermelho.\n");
    } 
    else if (escolha == 3) {
        printf("\nNa cena do crime você encontra uma luva vermelha.\n");
        printf("Ela parece ter impressões digitais.\n");
    } 
    else {
        printf("\nEscolha inválida.\n");
        return 0;
    }

    printf("\nApós juntar as pistas, quem você acha que é o culpado?\n");
    printf("1 - A esposa\n");
    printf("2 - O vizinho\n");
    printf("3 - Um ladrão desconhecido\n");
    printf("Escolha: ");
    scanf("%d", &escolha);

    if (escolha == 1) {
        printf("\nVocê acusa a esposa.\n");
        printf("Após análise, a luva encontrada tem as digitais dela.\n");
        printf("Parabéns! Você solucionou o caso!\n");
    } 
    else if (escolha == 2) {
        printf("\nVocê acusa o vizinho.\n");
        printf("Mas as provas não batem com ele. Caso não resolvido...\n");
    } 
    else if (escolha == 3) {
        printf("\nVocê acusa um ladrão qualquer.\n");
        printf("Mas não há provas suficientes. O assassino continua livre...\n");
    } 
    else {
        printf("\nEscolha inválida.\n");
    }

    printf("\n=== FIM DO JOGO ===\n");
    return 0;
}
