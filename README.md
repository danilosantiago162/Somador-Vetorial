Somador-Vetorial-EEL580
Este projeto implementa um somador vetorial em VHDL. O somador é capaz de realizar somas e subtrações de vetores de N bits em paralelo, onde N pode ser 4, 8, 16 ou 32 bits.

Descrição do Projeto
O projeto consiste em uma entidade VHDL chamada "SomadorVetorial". Essa entidade possui quatro portas de entrada e uma porta de saída:

Portas de Entrada:
A_i: Vetor de entrada A de N bits.
B_i: Vetor de entrada B de N bits.
vecSize_i: Tamanho do vetor, representado por um sinal de 2 bits.
mode_i: Modo de operação, onde '0' representa adição e '1' representa subtração.
Porta de Saída:
S_o: Vetor de saída de N bits, contendo o resultado da operação de soma ou subtração dos vetores A e B.
Implementação
O somador vetorial utiliza a lógica de complemento de 2 para realizar subtrações. Os sinais internos s_C e s_P são utilizados para gerar o carry antecipado necessário na operação de soma. O vetor B_op é usado para armazenar o complemento de 2 do vetor B, caso a operação seja uma subtração.

Após a geração dos carries antecipados, o somador realiza a soma bit a bit dos vetores A e B com o carry correspondente, gerando o vetor de saída S_o.

Autores
Este projeto foi desenvolvido por Carolina Santiago, Gustavo Roxo e Zuilho Segundo, como parte do trabalho para a disciplina Arquitetura de Computadores (EEL580) da UFRJ.
