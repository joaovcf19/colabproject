# colabproject
repositório colab
O código apresentado sobre morfologia, começa com a importação de bibliotecas para seu desenvolvimento, estas são: 
A biblioteca OpenCV, a qual é muito usada para processamento de imagens no caso deste código irá processa-las, para ser possível a sua manipulação e assim realizar a detecção de bordas da imagem.
E a biblioteca numpy a qual é renomeda como "np" através do comando "as np". A qual  é uma biblioteca usada para computação numérica em Python, que será necessária para este código para a criação da matriz 5x5 preenchida com numeros uns. 
Além disso é também é importada a função cv2_imshow para o google colab, a qual é uma modificação da função "cv2.imshow" da biblioteca OpenCV , modificação essa que permite que as imagens sejam exibidas diretamente no google colab. Isto irá ajudar a vizualizar a imagem processada ou não processada deste código ainda dentro do colab.
Após isso se da início ao carregamento de três imagens em escala de cinza e o armazenamento em suas respectivas variáveis, e a imagem armazenada na variável "img" terá suas dimensões de altura e largura obtidas pela função img.shape, dimensões as quais serão armazenadas em "altura, largura". 
Em seguida é criado um kernel, que é uma matriz 5x5 a qual é preenchida com numeros uns, essa matriz será usada como máscara ou estrutura que define a forma e o padrão de operação das transformações morfológicas, que ocorrerão na imagem como: erosão, gradinete,  dilatação, abertura e fechamento. Logo após isto a matriz é printada 
E então se da inicio nas próximas linhas do código o processamento das imagens sendo aplicadas seus "efeitos", estes são: erosão, gradinete,  dilatação, abertura e fechamento. 
O efeito de erosão irá ser utilizado para reduzir os detalhes da imagem, a dilatação para aumentar o tamanho dos objetos, o gradiente será utilizado para para realçar suas bordas, a abertura para remover ruuidos e objetos pequenos, e o fechamento para fechar pequenas aberturas.
E por fim será utilizado a função modificada pelo google colab "cv2_imshow" para exibir a imagem primeiramente de forma original, e depois será exibida a imagem após suas respectivas transformações de erosão, gradiente, dilatação, abertura e fechamento.
Desta froma pode-se concluir que o trecho de códigos apresentado consiste na aplicação de operações morfológicas com uma máscara de valores (kernel) na imagem como: Erosão, Gradiente, Dilatação, abertura e fechamento, para alterar justamente a composição da imagem, e assim fazendo com que a imagem após estas alterações, que será reproduzida pelo google colab através da função cv2_imshow, seja composta somente por bordas, ou seja, a imagem toda ficara preta, e aparecerá somente as bordas dos objetos ou pessoas. 
Este sistema de processamento de imagem também pode ser usado para sensores de presença onde identificam a presença das bordas do objeto ou pessoa, bem como nas tecnologias dos carros automáticos que utilizam sensores de aproximação e câmeras para identificar os obejtos a sua volta.
