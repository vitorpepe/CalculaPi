# CalculaPi - Sem Mutex

O programa começa pedindo ao usuário para digitar o número de threads que devem ser utilizadas no cálculo. É definindo um valor padrão para o número de iterações n = 1000000 = 10^6, e aloca memória para dois vetores: um para armazenar os identificadores das threads (thread_handles), e outro para armazenar as somas parciais calculadas por cada thread (sum).

O programa então inicializa o vetor de somas parciais com zero, cria as threads e as executa chamando a função Thread_sum para cada uma delas. A função Thread_sum recebe como parâmetro um índice de thread, e calcula a soma parcial correspondente a essa thread. A soma parcial é armazenada no vetor sum na posição correspondente ao índice da thread.

Após todas as threads terem concluído o processamento, o programa soma as somas parciais de todas as threads para obter o valor final de Pi, e multiplica o resultado por 4 para obter o valor correto. O programa imprime o valor final de Pi e libera a memória alocada para os vetores.



# CalculaPi - Com Mutex

