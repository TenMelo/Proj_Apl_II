# Proj_Apl_II
Repositório para registro da disciplina Projeto Aplicado II

# 1. INTRODUÇÃO
## 1.1. CONTEXTO DO TRABALHO
O ser humano desde sempre buscou contar histórias e eternizar momentos, e o que vemos hoje em dia com o amplo acesso à internet e, em especial, às redes sociais, nada mais é do que uma versão moderna do que já fazemos há mais de 50 mil anos, com as pinturas rupestres, quando começamos a manifestar nosso interesse em capturar momentos de conquistas ou aprendizados. Hoje em dia, a fotografia se tornou algo natural do nosso dia a dia, tanto pela facilidade da geração de conteúdo audiovisual proporcionado por nossos smartphones quanto pela facilidade de divulgação através das já mencionadas redes sociais. Aliando a fotografia ao esporte, temos a oportunidade de atingir nossos objetivos físicos e, também, a capacidade de reviver este momento sempre que quisermos, acessando as fotografias e filmagens do evento desejado

## 1.2. MOTIVAÇÃO E JUSTIFICATIVA
Surgirá, então, a necessidade de centralizar e organizar os registros de um evento esportivo. Vamos supor o seguinte cenário: uma corrida de pista fechada, como nas olimpíadas, com 10 atletas competindo em uma pista de 400 metros. Um evento rápido, com poucos atletas, e de muito simples organização dos arquivos, manualmente, inclusive. Imaginemos, agora, uma situação mais complexa: a cobertura de um Iron Man, uma prova de triatlo onde os atletas devem percorrer uma distância de 3.800 metros de natação, 180 Km de bicicleta e 42,195 Km de corrida, tudo isso sendo feito simultaneamente por mais de 1.700 atletas e sendo registrado por uma rede de 50 fotógrafos. Torna-se necessário, então, um algoritmo de classificação e agrupamento, para que o atleta possa buscar sua foto em um banco de dados através de métodos de pesquisa que sejam simples a ele, como seu número de inscrição ou uma foto do seu rosto.

Quem já participou de algum evento esportivo sabe a satisfação única de atingir e superar seus objetivos, e a possibilidade de eternizar este momento se torna possível à medida que este atleta consegue encontrar suas fotos em meio às demais, daí surge a necessidade de um algoritmo que possa identificar em uma foto a modalidade que está sendo praticada, como bicicleta ou corrida, identificar o atleta por seu número de inscrição - que normalmente é exigido estar em uma parte visível do corpo - via Optical Character Recognition (OCR), e ainda reconhecer seu rosto para que permitamos ao atleta buscar por suas fotos apenas enviando uma selfie, por exemplo.

Como exemplo, temos as empresas Foco Radical, Fotto e ClicRun, que já oferecem um serviço semelhante, mas não podemos, no entanto, utilizar seus repositórios devido à Lei Geral de Proteção de Dados (LGPD). Dessa forma, surge a possibilidade de utilizar incialmente o dataset Labeled Faces in the Wild, que conta com mais de 13.000 imagens de rostos devidamente identificados, em que ao menos 1.680 possuem duas ou mais fotos. Além disso, as imagens já estão devidamente rotuladas e separadas em conjunto de treinamento e verificação, servindo como base para um algoritmo inicial de reconhecimento facial.

## 1.3. OBJETIVOS
### 1.3.1. OBJETIVO GERAL:
Desenvolver um algoritmo que possibilite ao cliente encontrar de uma forma fácil e prática suas fotos em meio a um álbum de fotos de uma empresa, filtrando os elementos conforme lhe for conveniente.

### 1.3.2. OBJETIVOS ESPECÍFICOS:
1.	Agrupar as fotos via algoritmo de reconhecimento facial.
2.	Possibilitar um método de pesquisa reverso, onde o usuário irá enviar uma foto do seu rosto e terá como retorno suas fotos daquele respectivo álbum.
3.	Utilizar o OCR para leitura do número de identificação do atleta, se houver, para que também possa ser utilizado como parâmetro de pesquisa.
4.	Classificar as fotos conforme a sua modalidade desportiva.
5.	Possibilitar a interação entre os diversos filtros para uma busca precisa pelo usuário.
