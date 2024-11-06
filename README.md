# projeto-forca

Resumo do Projeto - Jogador de Forca Automático com Entropia
Este projeto implementa um jogador automático de forca que busca maximizar suas chances de vencer ao utilizar conceitos de teoria da informação, em particular o cálculo de entropia. O objetivo do jogador é descobrir a palavra secreta com o mínimo de erros, utilizando até cinco vidas. A cada nova partida, o jogador é informado sobre o número de letras da palavra, mas não tem acesso direto a ela, precisando adivinhar com base na resposta do "juiz", que indica a presença ou ausência da letra escolhida.

Estratégia e Conceitos Utilizados
O conceito central para a tomada de decisão é a entropia, uma medida da quantidade de informação associada a um evento, neste caso, à escolha de letras que reduzam a incerteza sobre a palavra secreta. A entropia mede a expectativa de redução na incerteza e é calculada para cada letra possível em cada estágio do jogo. Dessa forma, as letras com maior entropia são priorizadas, pois são mais prováveis de revelar informações sobre a palavra secreta.

Para calcular a entropia, o jogador avalia a frequência de cada letra no conjunto atual de palavras candidatas, ou seja, as palavras do vocabulário que têm o mesmo número de letras que a palavra-alvo e que não foram eliminadas em rodadas anteriores. A cada tentativa, o conjunto de palavras é filtrado conforme as respostas do "juiz" e, com isso, o jogador recalcula as probabilidades de cada letra aparecer em uma nova posição.

Desempenho e Avaliação
O desempenho do jogador é medido executando múltiplos jogos consecutivos e registrando a porcentagem de vitórias. Em simulações com um mínimo de 100 jogos, o jogador exibe a taxa de sucesso, oferecendo uma visão estatística da eficácia do algoritmo. A abordagem baseada em entropia garante uma taxa de sucesso elevada, pois permite que o jogador faça escolhas estratégicas com base na quantidade de informação provável a ser descoberta em cada etapa.

Conclusão
Esse projeto ilustra como o uso de entropia e teoria da informação, temas centrais em álgebra linear e ciência de dados, podem ser aplicados em um problema de descoberta. A técnica de entropia otimiza as escolhas do jogador, reduzindo erros e maximizando a chance de vitória. A implementação e avaliação deste algoritmo demonstram como métodos de informação teórica são poderosos na resolução de problemas de decisão.