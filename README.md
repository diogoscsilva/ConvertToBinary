Conversão de Imagem para Binário com Limiar Adaptativo
Este código executa a conversão de uma imagem colorida para uma imagem binária utilizando um limiar adaptativo. O limiar adaptativo é calculado com base no histograma da imagem em tons de cinza, o que permite que o limiar se ajuste a diferentes condições de iluminação e contraste na imagem.

Bibliotecas:

numpy para manipulação de arrays e imagens.
Pillow para abrir e manipular imagens.
matplotlib para exibir imagens.

 Os valores em tons de cinza são adicionados ao histograma.
O valor limite é calculado usando uma fórmula que leva em consideração 50% da frequncia acumulada dos pixels em nível de cinza do histograma, e é feito um ajuste em direção ao valor médio de cinza (128).

Se o valor do pixel for menor que o limiar, o pixel correspondente em binary_img é definido como 0 (preto).
Caso contrário, o pixel correspondente em binary_img é definido como 255 (branco).
