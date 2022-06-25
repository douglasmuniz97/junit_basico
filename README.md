# junit_basico

@Test Métodos com esta anotação serão identificados como teste para a execução

O método do teste deve ser publice void

Execução do Erro:
SUcesso: quando o teste executa com sucesso. cor verde
Erro: Quando algum erro de lógica ou esceção ocorre. cor vermelha
Falha: QUando uma falaha na validação de resultados ocorre. cor azul.

Assert: Irá nos dar a certeza do resultado apresentando um resultado positivo ou negativo

assertTrue e False: validar um retorno verdadeiro ou falso

assertEquals faz a comparação do resultado esperado e do resultado obtido e mostra o sucesso a falha

@Before: é uma pré condição no metodo que sera executado antes do teste, before tambem pode ser conhecido om setup

@After: é uma pós condição no método que será executado após o teste, tambem pode ser conhecida como teardown.

@BeforeClass: executa alguma ação antes da execução da classe de teste, e deve ser sem retorno static

@AfterClass: executa alguma ação depois que todos os teste ja tenham sido executados, e deve ser sem retorno static

@RunWith: anotação que deve ser colocada acima da classe que irá disparar diversos testes, deve ter o paramentro Suite.class.

@SuiteClasses: anotação que deve ser colocado acima da classe, que irá informar quais os testes serão executados. Dentro dos {} deve ter os nomes das classes.

@Parameters: fica acima do método e informa os arrays com os dados que serão usados no data driven

@FileParameters: caminho e especificações do arquivo csv. Value: o caminho onde se encontra o arquivo csv. mapper: informa que tem um cabecalho no csv.

@Igonore: faz com que o teste não seja executado, pode ser inserido antes ou depois do @test. pode colocar o value dentro do ignore e colocar um comentario do motivo da ignoração.

@Timeout: adiciona um tempo para que o teste seja executado. tambem pode ser usado no before e after. timeout vai dentro de @Rule.


 --------GRUPO ASSERTHAT-----
assertThat: garanta que alguma coisa é tambem alguma coisa.

equalTo: Valida se um resultado obtido é igual ao esperado com tipo caracter.

is: semelhante ao euqalTo, mas se usa com tipos numéricos.

anyOf + containsString: Valida se um resultado esperado esta contido em um texto ou array.

hasItem: Valida se um item existe em um array de objetos.
--------------------------

@IncludeCategory: realiza uma separação de testes por categoria, exemplo: smoke, positivo e negativo. Tem que ser criado interfaces nas categorias
Smoke: testes muito importantes
Positivo: testes que terão sucesso.
Negativo: testes que não terão sucesso.
