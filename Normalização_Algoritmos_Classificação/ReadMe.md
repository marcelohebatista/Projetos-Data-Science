# Normalização 

É uma das primeiras tarefas dentro do pré-processamento, ou seja, colocar seus dados na mesma escala. 

Muitos algoritmos de Machine Learning irão se beneficiar com esse processo e produzirão melhores resultados. 

Os arquivos jupyter notebook produzidos fornecerão exemplos práticos utilizando alguns métodos, com alguns algoritmos de classificação.

Instruções e links de utilização.

1) Utilize o shell [clear_files.sh] para limpar os arquivos .csv e .png 

2) Utilize o shell [run_all_ipynb.sh], pois existe uma sequência para a construção do produto final no arquivo [resultados/resultados.csv]

3) Abaixo a relação dos arquivos jupyter notebook que serão utilizados:

- Sem_Normalizacao.ipynb
- Normalizacao_Binarizer.ipynb
- Normalizacao_MinMaxScaler.ipynb
- Normalizacao_Normalizer.ipynb
- Normalizacao_StandardScaler.ipynb

4) Links para os métodos utilizados do scikit-learn

## Binarizer 

Podemos definir um valor em nossos dados, ao qual chamamos de threshold, ou seja, definimos que todos os valores acima de um determinado valor será marcado como sendo 1 e todos valores iguais ou abaixo deste threshold serão marcados como sendo 0. 
Também chamado de Binarização. Sendo útil quando temos probabilidades e queremos transformar os dados em algo com mais significado. No scikit-learn a função é chamada de Binarizer().

https://scikit-learn.org/stable/modules/generated/sklearn.preprocessing.Binarizer.html  

## MinMaxScaler 

Chamada de normalização que coloca os dados em uma escala entre 0 e 1. Sendo muito para  otimização, sendo usado no core dos algoritmos de Machine Learning, como gradient descent. 
Muito útil para algoritmos como regressão e redes neurais e algoritmos que usam medidas de distância, como KNN. O scikit-learn possui a chamada MinMaxScaler().

https://scikit-learn.org/stable/modules/generated/sklearn.preprocessing.MinMaxScaler.html  

## Normalizer 

Método utilizado para o pré-processamento é útil quando temos datasets esparsos (com muitos zeros) e atributos com escala muito variada. Mostra utilizade quando usamos algoritmos de redes neurais ou que usam medida de distância, como KNN. O scikit-learn possui a chamada Normalizer().

https://scikit-learn.org/stable/modules/generated/sklearn.preprocessing.Normalizer.html 

## StandardScaler

Essa técnica serve para transformar os atributos com distribuição Gaussiana (normal) e diferentes médias e desvios padrão em uma distribuição Gaussiana com a média igual a 0 e desvio padrão igual a 1. 
Isso é útil para algoritmos que esperam que os dados estejam com uma distribuição Gaussiana, como regressão linear, regressão logística e linear discriminant analysis. Funciona quando os dados já estão na mesma escala. O scikit-learn possui a chamada StandardScaler().

https://scikit-learn.org/stable/modules/generated/sklearn.preprocessing.StandardScaler.html


5) Não temos como saber qual algoritmo vai funcionar da melhor forma com os nossos dados. Precisamos testar com alguns algoritmos nosso dataset. Para tanto iremos testar nosso conjunto de dados com os Algoritmos de Machine Learning listados abaixo:

- LR - Logistic Regression
- KNN - K Nearest Neighbors
- CART - Classification and Regression Trees
- SVM -  Support Vector Machines
- RF - Random Forest
