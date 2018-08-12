# Algoritmo de Ordenação Insertion Sort
Algoritmo que mede a interação para ordenar vetores (crescente e decrescente) e desordenados, ele mede o número de interações.

O algoritmo tem como principal caracteristica manter duas interações de ciclos de repetição. Onde é elegido um "pivo" para fazer a comparação com o valor anterior. Se o valor do vetor comparado com o "pivo" for menor que o pivo, o algoritmo deve fazer a troca de lugares para ordenar o vetor de forma crescente, caso ele não seja menor o algoritmo deve quebrar a interação do ciclo de repetição interno (pois os valores podem ja vir odenados assim nao sendo necessario fazer todas as comparações novamente.). 


## Desempenho do algoritmo

O algoritmo em si se utiliza de seus meios de comparação para ordenar o vetores, mas além das suas linhas de código ele depende muito do tamanho dos arrays recebidos e se eles estao ordenados ou não. No exemplo da imagem abaixo eu utilizei um array com 10 posições, um ordenado de forma Crescente, um Decrescente e um Desordenado (Aleatório). Esses arrays representam o melhor, pior e caso médio que este algoritmo pode apresentar em termos de número de interações necessarias para se fazer a ordenação.

![enter image description here](https://lh3.googleusercontent.com/cDAze2FnguI7o4qW-ZondbSanm6gPMpfysn1k8ibS9xKiYU1lljYCp6uFVrlHxopztxUUV990zPILg "Vetores ordenados com insertion Sort")

## Testes de desempenho

Agora fazendo os mesmos testes com vetores de 1 a 100, gerados com valores Crescentes, Decrescentes e Aleatorios, fazendo com que o algoritmo escrevece a quantidade de interações feitas com cada tipo de vetor, conseguimos retirar um gráfico no Br Office Calc e obtemos os seguintes resultados apresentados no gráfico a seguir.

![enter image description here](https://lh3.googleusercontent.com/-iLrcI6gkvAGeV87IGZMsedY2MiQO2YIcJvK7y2-Ao9NG5LnoOtObBPGNTUej0A3Nh-3MVPh93_dqA "InsertionSort")

É importante notar como no melhor caso, (com um vetor já ordenado) o algoritmo não apresenta um número alto de interações.

## Comparação do Algoritmo InsertionSort com o SelectionSort e o BubbleSort (versao 1 e 2)

Como apresentado no gráfico abaixo temos o numero de interações que cada um dos algoritmos nos trás, estando no pior caso, caso médio ou pior caso, independente do tamanho do array ele sempre cresce de uma forma exponencial. O gráfico mostra de uma forma mais clara o seu número de interações.

![enter image description here](https://lh3.googleusercontent.com/DMlOWUaAyZUn0_UsrZ4KHB7BFi8t3wLWzz3b73DMPJPoof62K_D8OEsXuPTK12K4hkpUuLDRr75yng "Comparação de desempenho Insertion Sort")

Aqui podemos observar que o pior caso do InsertionSort é ainda pior que os demais algoritmos já estudados até então. E vemos que o melhor caso dele é bem equivalente (segue a formula vetor tamanho N interaçoes ((N*2) - 2) ao melhor caso do BubbleSort2

## Sobre o trabalho

Os dados utilizados para gerar o gráfico são do retorno do algoritmo criado neste projeto. O arquivo CSV utilizado para a criação do gráficos se encontra dentro da pasta "src".

## Execução
No código da Classe MainCSV na linha 15, existe uma tag que deve ser mudada para gerar o arquivo CSV, ali eu especifiquei uma pasta do meu ambiente de trabalho no Ubuntu, mas deve-se trocar o local de criação do arquivo.

Após a execução do algoritmo e receber a mensagem de "Arquivo CSV criado com Sucesso!" o seu arquivo CSV é criado. E com ele eu criei o gráfico da imagem acima.