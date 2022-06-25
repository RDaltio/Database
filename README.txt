Extraia a pasta .zip e obterá uma pasta chamada BD2, dentro dela existe este arquivo README, um arquivo "iris.data", um arquivo PDF do relatório, slides para visualização do código e uma pasta com nome TRABALHO2 que contém os arquivos txt a serem utilizados.
Cole a pasta "BD2" no disco C, ficando com o seguinte endereço a ser usado posteriormente: 

'C:\BD2\iris.data'

Para o código do projeto:

1-) Primeiramente abra o arquivo txt Tables e cole o código de criação da tabela "plant".

2-) Após sua criação será necessário utilizar o database cedido pelo professor para inserir os dados na tabela.
Para isso utiliza-se o código 2-) do arquivo txt Functions.
É preciso que o arquivo com os dados esteja na pasta com endereço utilizado na linha 10 deste arquivo txt.
Pode-se escolher a pasta do arquivo dos dados, porém seu endereço deve ser colado no valor da linha 12 do arquivo txt Functions.

3-) Tendo os dados inseridos cria-se a tabela "training" com o código 3-) do arquivo txt Tables.

4-) Tendo os dados inseridos cria-se a tabela "sample" com o código 4-) do arquivo txt Tables.

5-) Tendo os dados inseridos cria-se a tabela "distance" com o código 5-) do arquivo txt Tables.

6-) Cria-se a as visões das classes de plantas setosa, versicolor e virginica utilizando o código 6-) do arquivo txt Views.

7-) É criada a função de treinamento utilizando o código 7-) do arquivo txt Functions.

8-) Por fim cria-se a função k-nearest neighbors com o código 8-) do arquivo txt Functions.

Tendo todo o código montado, basta chamar as funções com o script:

SELECT sampleTraining(); 
--Utilizamos uma porcentagem de 70% para treino e 30% para amostras.
 
e posteriormente:

SELECT knn(k); 
--onde k é o valor de vizinhos desejados na comparação, caso não utilize parametros o valor de k está como default = 1.

Por fim para facilitar a visualização utilize o comando a seguir com o parametro k da mesma forma como mencionado acima:

SELECT * FROM knn(k);

Dessa forma o código estará completo e entregando a tabela de saída desejada, comparando os k vizinhos.

A qualquer momento pode-se fazer o uso do comando a seguir para verificar o andamento do código, desde que sua criação já tenha sido efetuada:

SELECT * FROM <nome da tabela/nome da view>;
