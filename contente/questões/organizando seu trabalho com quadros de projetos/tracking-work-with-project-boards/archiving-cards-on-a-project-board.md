---
title: Archiving cards on a project board
intro: You can archive project board cards to declutter your workflow without losing the historical context of a project.
redirect_from:
  - /github/managing-your-work-on-github/tracking-the-progress-of-your-work-with-project-boards/archiving-cards-on-a-project-board
  - /articles/archiving-cards-on-a-project-board
  - /github/managing-your-work-on-github/archiving-cards-on-a-project-board
versions:
  free-pro-team: '*'
  enterprise-server: '*'
  github-ae: '*'
topics:
  - Pull requests
---
Automation in your project board does not apply to archived project board cards. For example, if you close an issue in a project board's archive, the archived card does not automatically move to the "Done" column. When you restore a card from the project board archive, the card will return to the column where it was archived.

### Archiving cards on a project board

1. In a project board, find the card you want archive, then click {% octicon "kebab-horizontal" aria-label="The horizontal kebab icon" %}.
![List of options for editing a project board card](/assets/images/help/projects/select-archiving-options-project-board-card.png)
2. Click **Archive**.
![Select archive option from menu](/assets/images/help/projects/archive-project-board-card.png)

### Restoring cards on a project board from the sidebar

{% data reusables.project-management.click-menu %}
2. Click {% octicon "kebab-horizontal" aria-label="The horizontal kebab icon" %}, then click **View archive**.
  ![Select view archive option from menu](/assets/images/help/projects/select-view-archive-option-project-board-card.png)
3. Above the project board card you want to unarchive, click **Restore**.
  ![Select restore project board card](/assets/images/help/projects/restore-card.png)
include <string.h>

//Constantes

#define tamanho 5

//Estrutura  

struct taluno {

int ra;

int matricula;

char arquivo[50];

char extensao[50];

 

};

//Estrutura da Pilha

struct tpilha {

taluno dados[tamanho];

int ini;

int fim;

};

//Variáveis globais

tpilha pilha;

//Adicionar um elemento no final da Pilha

void pilha_entrar(){

if (pilha.fim == tamanho) {

 

printf("\nA pilha está cheia, impossível empilhar!\n\n");

system("pause");

}

else {

printf("\nDigite o RA do aluno: ");

scanf("%d", &pilha.dados[pilha.fim].ra);

printf("\nDigite o nome do Arquivo: ");

scanf("%s", pilha.dados[pilha.fim].arquivo);

printf("\nDigite a extesao do Arquivo: ");

scanf("%s", pilha.dados[pilha.fim].extensao);

printf("\nDigite a matricula do Professor: ");

scanf("%s", pilha.dados[pilha.fim].matricula);

pilha.fim++;

}

}

//Retirar o último elemento da Pilha

void pilha_sair() {

if (pilha.ini == pilha.fim) {

printf("\nA pilha está vazia, impossível desempilhar!\n\n");

system("pause");

}

else {

pilha.dados[pilha.fim-1].ra = 0;

strcpy(pilha.dados[pilha.fim-1].ra, "");

strcpy(pilha.dados[pilha.fim-1].arquivo, "");

pilha.fim--;

}

}

//Mostrar o conteúdo da Pilha

void pilha_mostrar() {

int i;

printf("[ ");

for (i = 0; i < tamanho; i++) {

printf("%d ", pilha.dados[i].ra);

}

printf("]\n\n");

}
