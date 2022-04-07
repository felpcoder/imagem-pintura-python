# Transformando imagem em pintura com Python e Opencv

A ideia central desse projeto é transformar uma fotografia em uma imagem com aspectos de pintura. Para isso será usada a linguagem de programação Python e as bibliotecas Opencv, Sklearn e Numpy. Todo o código está disponível no arquivo Painting_image.ipynb, e as imagems correspondem as fases do processamento descritas abaixo.

Primeiro é feita a leitura da imagem. A seguir, faremos processamento tanto com a imagem original colorida, quanto com a imagem original em tons de cinza. Por fim, combinaremos as duas imagens para termos o resultado.

O processamento da imagem colorida consiste em fazer uma quantização de cores, usando o algoritmo k-means, para dar um aspecto mais homogêneo as cores da imagem. Depois disso, aplicamos um filtro de média.

O processamento em tons de cinza, começa transformando a imagem original em uma imagem em tons de cinza. Após isso, é aplicado um filtro de média. Com o resultado, aplicamos o algoritmo Canny Edges Detection para detectar as bordas da figura, aplicamos uma operação morfológica de dilatação para ampliar as bordas da imagem e em seguida invertemos as cores do resultado. 

Para combinar os dois processamentos. Usamos a imagem colorida processada com a imagem em tons de cinza processada para gerar uma imagem com os contornos coloridos. Por fim juntamos essa última imagem, com o resultado do processamento colorido. 

# Imagem original e Resultado após o processamento completo
![img_antes_depois](https://user-images.githubusercontent.com/74699523/162235955-b68f9fe9-19d4-49af-880c-953a38d335a9.png)
