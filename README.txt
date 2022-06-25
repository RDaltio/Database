Este foi meu projeto para a matéria Banco de Dados 2, onde por meio da implmentação do algoritmo dos k viznhos as plantas dos dados fornecidos pelo professor poderiam estar classificadas de forma equivocada. Para isso criei as funções e as tabelas, inseri os dados e foram calculadas as novas classificações das plantas. Esse projeto foi feito no PostgreSQL.
Neste arquivo ensino como rodar essa aplicação, ela foi dividida conforme o pedido do professor de Banco de Dados 2, neste repositório contém um arquivo "iris.data" e os arquivos txt a serem utilizados.
Crie uma pasta "BD2" e cole todos os arquivos txt dentro dela.
Cole a pasta "BD2" no disco C, ficando com o seguinte endereço a ser usado posteriormente: 

'C:\BD2\iris.data'

Para o código do projeto:

1-) Primeiramente abra o arquivo txt Tables e cole o código de criação da tabela "plant".

2-) Após sua criação será necessário utilizar o database cedido pelo professor para inserir os dados na tabela.
Para isso utiliza-se o código 2-) do arquivo txt Functions.
É preciso que o arquivo com os dados esteja na pasta com endereço utilizado na linha 6 deste arquivo txt.
Pode-se escolher a pasta do arquivo dos dados, porém seu endereço deve ser colado no valor da linha 6 do arquivo txt Functions.

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
