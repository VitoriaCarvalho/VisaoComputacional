# Visão Computacional

Um pouco dos trabalhos desenvolvidos durante a disciplina de Visão Computacional, do curso de Sistemas de Informação. Todos os trabalhos foram implementados na linguagem Python e escritos usando o JupyterLab do Anaconda.

---

## :computer: Detalhes dos algoritmos:

A seguir, está uma breve explicação sobre cada um dos trabalhos:

* <a href="https://github.com/VitoriaCarvalho/VisaoComputacional/blob/master/Trabalho%201%20-%20Manipulando%20Imagens/manipulandoImgs.ipynb">Trabalho 1 - Manipulando imagens</a>
<br>Neste trabalho, aprendemos como realizar manipulações simples em imagens, como por exemplo leitura, escrita, conversão para níveis de cinza, separação de canais, iteração entre os pixels, etc. Em seguida, testamos alguns tipos de ruídos, filtros e detectores de borda. Por fim, aprendemos a fazer cortes nas imagens sem utilizar métodos prontos.

* <a href="https://github.com/VitoriaCarvalho/VisaoComputacional/blob/master/Trabalho%202%20-%20Histogramas/histogramas.ipynb">Trabalho 2 - Histogramas</a>
<br>Neste trabalho, utilizamos uma base de frutas (disponibilizada no repositório) para a implementação de histogramas. Implementamos 6 atributos para caracterizar os histogramas: mean, variance, skewness, kurtosis, energy e entropy.  Dessa forma, para cada uma das imagens de maçãs e tomates (que são das duas classes da base), foi gerado um histograma e calculados os atributos implementados. Por fim, plotamos algumas combinações dos atributos para analisar a relevância dos mesmos na tendência de separabilidade das classes.

* <a href="https://github.com/VitoriaCarvalho/VisaoComputacional/blob/master/Trabalho%203%20-%20Transforma%C3%A7%C3%A3o%20de%20Intensidade%20e%20Quantiza%C3%A7%C3%A3o%20de%20Imagens/transf_intensidade.ipynb">Trabalho 3 - Transformações de Intensidade</a>
<br>Neste trabalho, implementamos as seguintes transformações de intensidade: alargamento de contraste, negativa, logarítmica e potência. Ao aplicar as transformações às imagens, plotamos os resultados variando os parâmetros das funções, a fim de analisar o impacto dos mesmos nas modificações visuais das imagens. Em seguida, implementamos o fatiamento por planos
de bits, que permite analisar a importância relativa de cada bit na imagem, podendo ajudar a definir o
número adequado de bits para quantizar uma imagem.

* <a href="https://github.com/VitoriaCarvalho/VisaoComputacional/blob/master/Trabalho%204%20-%20%09Filtragem%20Espacial/filtragem_espacial.ipynb">Trabalho 4 - Filtragem Espacial</a>
<br>Neste trabalho, aprendemos a implementar filtros espaciais, que são utilizados para borrar imagens e reduzir ruídos, sendo bastante aplicados na etapa de pré-processamento de imagens. Aplicamos os filtros utilizando convoluções, onde o filtro é passado em cada kernel da imagem, sendo que o pixel central de cada kernel receberá a somatório da multiplicação ponto a ponto do filtro pelo kernel. Para este processo de convolução, é necessário realizar um tratamento na borda, para garantir que o kernel não passará da imagem. Os tratamentos de borda implementados foram: ignorar a borda, preencher com zeros,
replicar e espelhar. Dentre os filtros aplicados, o da mediana é comumente utilizado para redução de ruídos nas imagens.

* <a href="https://github.com/VitoriaCarvalho/VisaoComputacional/blob/master/Trabalho%205%20-%20Segmenta%C3%A7%C3%A3o/segmentacao.ipynb">Trabalho 5 - Segmentação</a>
<br>Neste trabalho, utilizamos uma base de folhas (disponibilizada no repositório) para testar os algoritmos k-means, otsu e superpixel na tarefa de segmentação das imagens. Ao final do trabalho, aplicamos 3 métricas de validação para avaliar as segmentações geradas pelos algoritmos. O kmeans e otsu mostraram-se eficientes nesta tarefa, já que existe uma heterogeneidade evidente na imagem em relação à intensidade dos pixels. O superpixel, por sua vez, não conseguiu separar as regiões com êxito, já que na maioria nas imagens agrupou todos os pixels em um só cluster.

* <a href="https://github.com/VitoriaCarvalho/VisaoComputacional/blob/master/Trabalho%206%20-%20Processamento%20de%20Imagens%20Coloridas/transformacao_de_cores.ipynb">Trabalho 6 - Processamento de Imagens Coloridas</a>
<br>Neste trabalho, utilizamos o processamento em pseudocores a partir do fatiamento de intensidade. A aplicação escolhida para testar o fatiamento de intensidades foi a análise de lesões de pele para detecção de melanoma. A partir do fatiamento de cores, foi possível separar a lesão da pele e destacar as regiões que demonstram ser suspeitas da existência de um melanoma. Em seguida, o algoritmo de convolução implementado no trabalho 4 foi adaptado para processar imagens coloridas. Por fim, testamos os algoritmos k-means, otsu e mini batch k-means em diferentes modelos de cores. Os modelos de cores utilizados foram o CMY, o HSV e o YUV, sendo que o melhor resultado foi obtido pelo componente C do modelo CMY, na segmentação com o otsu.

* <a href="https://github.com/VitoriaCarvalho/VisaoComputacional/blob/master/Trabalho%207%20-%20Extra%C3%A7%C3%A3o%20de%20Caracter%C3%ADsticas%20-%20Descritor%20HOG/descritor_hog.ipynb">Trabalho 7 - Descritor HOG</a>
<br>Neste trabalho, implementamos o algoritmo histogram of oriented gradients (HOG), utilizado para extrair características das imagens. O HOG pode ser representado de várias formas, sendo que alguns consideram apenas a orientação, outros apenas a magnitude e outros os dois. Dessa forma, optamos por retornar dois histogramas na nossa função, um de orientação e outro de magnitude. O embasamento para a implementação dos métodos foi obtido com as explicações apresentadas <a href="https://www.analyticsvidhya.com/blog/2019/09/feature-engineering-images-introduction-hog-feature-descriptor/">neste site</a>.

---

## :memo: Licença

Esse projeto está sob a licença MIT. Veja o arquivo [LICENSE](https://github.com/VitoriaCarvalho/VisaoComputacional/blob/master/LICENSE) para mais detalhes.

---

Algoritmos desenvolvidos por [Vitória Carvalho](https://www.linkedin.com/in/vit%C3%B3ria-carvalho-90210b19a/) :woman::computer:
