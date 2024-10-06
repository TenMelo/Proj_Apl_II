# Proj_Apl_II
# 1. INTRODUÇÃO
## 1.1. CONTEXTO DO TRABALHO
No cenário atual de rápida evolução tecnológica, a geração de imagens por meio de inteligência artificial tem se tornado uma ferramenta essencial em diversas áreas, desde o design gráfico até a criação de conteúdo digital. O MidJourney, uma plataforma inovadora de geração de imagens, tem se destacado por sua capacidade de produzir imagens de alta qualidade de maneira eficiente. No entanto, como qualquer tecnologia emergente, há sempre espaço para melhorias.

Este projeto tem como objetivo principal o aprimoramento do processo de geração de imagens do MidJourney. Através de uma análise detalhada dos métodos atuais e da implementação de novas técnicas, buscamos aumentar a precisão, a velocidade e a qualidade das imagens geradas, tornando-a ainda mais versátil e útil para seus usuários.

Para fins de comparação e conclusão do projeto, exibiremos imagens geradas pelo MidJourney ao lado de imagens aprimoradas pelo nosso sistema. Essa abordagem permitirá uma análise clara das diferenças e destacará as melhorias alcançadas, assegurando uma conclusão robusta e bem fundamentada do projeto.

A seguir, serão apresentados os principais desafios enfrentados atualmente, as metodologias propostas para superá-los e os resultados esperados com a implementação das melhorias sugeridas. Este documento servirá como um guia detalhado para todas as etapas do projeto, garantindo uma abordagem estruturada e eficiente para alcançar nossos objetivos.
## 1.2. OBJETIVOS
A geração de imagens pelo MidJourney enfrenta vários desafios, que podem ser categorizados em técnicos e de usabilidade. Entre os pontos mais críticos que identificamos estão:

1.	Precisão e Realismo

a.	Detalhamento Realista: Embora o MidJourney tenha melhorado significativamente, ainda pode ser difícil gerar imagens com um nível de detalhe realista consistente, especialmente em contextos complexos.

b.	Texto Legível: A inclusão de texto claro e legível nas imagens é um desafio contínuo. Versões anteriores frequentemente produziam caracteres distorcidos ou sem sentido.

2.	Interpretação de Prompts

a.	Compreensão da Linguagem Natural: A ferramenta precisa interpretar corretamente os prompts fornecidos pelos usuários. Isso pode ser complicado, pois requer uma compreensão precisa da linguagem natural e das nuances dos comandos1.

b.	Especificidade dos Prompts: Usuários precisam ser muito específicos em seus comandos para obter os resultados desejados, o que pode ser uma barreira para aqueles menos familiarizados com a ferramenta2.

3.	Consistência e Coerência

a.	Manutenção da Consistência: Manter a consistência em iterações de personagens ou estilos ao longo de várias imagens é um desafio, especialmente quando se utiliza modelos de difusão que geram imagens pixel por pixe.

Para alcançar o objetivo de aprimorar o processo de geração de imagens do MidJourney, elaboramos um plano estruturado que abrange várias etapas. Sendo assim:

1.	Análise do Estado Atual

a.	Revisão dos Métodos Atuais: Avaliar as técnicas e algoritmos atualmente utilizados pelo MidJourney para identificar pontos fortes e fracos.

2.	Definição de Metas e Objetivos

a.	Qualidade das Imagens: Estabelecer padrões de qualidade que as novas imagens devem atingir.

3.	Pesquisa e Desenvolvimento

a.	Exploração de Novos Algoritmos: Pesquisar e testar novos algoritmos de inteligência artificial que possam melhorar a geração de imagens.

b.	Implementação de Técnicas de Aprendizado Profundo: Utilizar redes neurais profundas e outras técnicas avançadas de aprendizado de máquina para aprimorar a precisão e a qualidade das imagens.

4.	Prototipagem e Testes

a.	Desenvolvimento de Protótipos: Criar protótipos das novas soluções e funcionalidades para testes iniciais.

b.	Testes de Qualidade: Realizar testes rigorosos para garantir que as novas soluções atendam aos padrões de qualidade estabelecidos.

## 1.3 DEFINIÇÃO DAS LINGUAGENS UTILIZADAS
Neste projeto será utilizada a linguagem Python por se tratar de uma linguagem amplamente usada no meio da ciência da computação para aprendizado de máquina, projetos que envolvem Deep Learning, entre outros exemplos, o que além a tornarem uma ferramenta eficaz, faz com existam diversos repositórios de código que contribuem para o desenvolvimento de outros projetos.
## 1.4 BASE DE DADOS
A base de dados utilizada será uma base do site ImageNet, também disponível no Kaggle, ofertada pela Princeton University e Stanford University, que se trata de uma série de imagens rotuladas que servirão tanto para o treinamento do modelo que irá entender a imagem através de visão computacional, para que assim possa decodificá-la, quanto para a possível geração de imagens melhores que as fornecidas pelo MidJourney, pelos parâmetros elaborados anteriormente.
## 1.5 CRONOGRAMA
Etapa 1 – Começo do Projeto
Atividades e Prazos:

•	(26/08/2024) Semana 1:

o	Definir o grupo de trabalho.

o	Definir as premissas do projeto: empresa, área de atuação e dados (imagem ou texto).

•	(02/09/2024) Semana 2:

o	Determinar objetivos e metas.

o	Criar um cronograma de atividades.

Etapa 2 – Definição do Produto Analítico
Objetivos: Análise exploratória da base de dados e definição do método analítico.
Atividades e Prazos:

•	(09/09/2024) Semana 3:

o	Definir bibliotecas (pacotes) Python e repositório no GitHub.

o	Definir a base de dados e iniciar a análise exploratória.

•	(16/09/2024) Semana 4:

o	Tratar a base de dados (preparação e treinamento).

o	Definir e descrever as bases teóricas dos métodos analíticos.

•	(23/09/2024) Semana 5:

o	Definir e descrever como será calculada a acurácia.

Etapa 3 – Apresentação de Produtos e Storytelling
Objetivos: Consolidação dos resultados e preparação para apresentação.
Atividades e Prazos:

•	(30/09/2024) Semana 6:

o	Consolidar os resultados do método analítico.

o	Aplicar as medidas de acurácia.

•	(14/10/2024) Semana 7:

o	Descrever os resultados preliminares e apresentar um produto gerado.

o	Descrever um possível modelo de negócios.

•	(21/10/2024) Semana 8:

o	Esboçar o Storytelling.

Etapa 4 – Apresentação e Conclusão do Projeto
Objetivos: Finalizar e apresentar o projeto.
Atividades e Prazos:

•	(04/11/2024) Semana 9:

o	Preparar a apresentação final.

o	Revisar e ajustar o Storytelling.

•	(18/11/2024) Semana 10:

o	Apresentação final do projeto.

# 2. DESENVOLVIMENTO
## 2.1 TRATAMENTO DA BASE DE DADOS
A fim de começar o projeto de uma forma mais simplificada, iremos reduzir a nossa base de dados para imagens que contenham mãos e textos para que possamos focar na melhoria destes itens, conforme mencionado anteriormente, e assim ir desenvolvendo o restante do projeto ao longo do tempo. Desta forma, será necessário limpar a base de dados para selecionar apenas as imagens relevantes ao projeto, ao que estas serão divididas aleatoriamente e categorizadas em treinamento e teste, com uma proporção aproximada de 4:1.
## 2.2 DEFINIÇÃO E DESCRIÇÃO DAS BASES TEÓRICAS DOS MÉTODOS
Fundamentos Matemáticos da Geração de Texto:

A base da geração de texto por Inteligência Artificial Generativa (IAG) reside em modelos de linguagem, como os Transformers, que utilizam redes neurais artificiais para aprender padrões complexos em grandes conjuntos de dados textuais. 

O Transformer é um tipo de arquitetura de rede neural que se destaca por sua habilidade em processar sequências de dados, como texto, código ou até mesmo áudios, gerando uma hierarquia de importância através do seu mecanismo de attention (atenção) entre palavras soltas ou pequenos trechos de texto do prompt de entrada. 

O processo de geração de resposta ocorre nas seguintes etapas: 

•	Codificação do Prompt: O prompt fornecido pelo usuário é transformado em uma representação numérica, geralmente utilizando técnicas de embedding. Essa representação captura o significado semântico e sintático das palavras. 

•	Stemming (Derivação): O modelo analisa as partes do prompt transformadas em números para descobrir o que a sentença está dizendo

•	Análise de dependência: O algoritmo descobre como as palavras da sentença estão relacionadas, geralmente utilizando árvores de decisão com uma única palavra como raiz (geralmente verbos)

•	Decodificação: A rede neural decodifica a representação numérica do prompt, gerando uma sequência de palavras prováveis. A cada passo, o modelo considera as palavras já geradas e o prompt original para prever a próxima palavra, através de probabilidades estatísticas gerada das fases anteriores 

Papel dos Parâmetros do Prompt:

Cada palavra no prompt influencia a geração da resposta de maneira distinta. Palavras-chave (geralmente verbos, substantivos e adjetivos) direcionam a geração para tópicos específicos, enquanto a ordem das palavras e a estrutura da frase influenciam a sintaxe e a coesão do texto. Além disso, parâmetros como o comprimento máximo da resposta podem ser ajustados para controlar a criatividade e a coerência do texto gerado. 

Processamento de Imagens:

A geração de imagens por IAG segue a mesma estrutura do PLN explicada anteriormente, utilizando o resultado desse processo como input para o algoritmo gerador de imagens, possuindo apenas uma camada adicional de processamento e treinamento com dados rotulados, visando o entendimento das características fundamentais que definem o objeto, ou seja, o que diferencia algo de outro.

Processamento de Arquivos:

O processamento de arquivos de imagem envolve a conversão das imagens em um formato numérico que possam ser processados corretamente, onde as imagens são convertidas em matrizes numéricas onde cada número representa um pixel da imagem. A escolha do formato de arquivo (JPEG, PNG etc.) e a resolução da imagem influenciam a qualidade da representação numérica.
## 2.3 DEFINIÇÃO E DESCRIÇÃO DA ACURÁCIA
A acurácia será calculada através de um método simples de verificação pela base de dados de teste, onde é possível verificar a taxa de acertos e também através do uso de Optical Character Recognition (OCR), ferramenta consolidada desenvolvida para leitura de textos em imagens, que deverá identificar se há algo escrito na imagem e comparar a semântica com a de um dicionário de referência, onde será por fim calculada a acurácia pela taxa de correspondência entre os caracteres gerados e lidos com os do anteriormente mencionado dicionário.

 
# REFERENCIAS: 

LI, Y.; LIU, B.; XIE, L. Dimensionality reduction for clustering. Journal of Machine Learning Research, v. 21, p. 1-28, 2020. 

RENDLE, S. et al. Factorization machines. In: 2010 IEEE International Conference on Data Mining. Proceedings… Sydney, Australia: IEEE, 2010. p. 995-1000. 

SAMMUT, C.; WEBB, G. I. Encyclopedia of Machine Learning. New York: Springer, 2011. 

Ricci, F., Rokach, L., & Shapira, B. (2015). Recommender Systems Handbook. Springer. 

Jolliffe, I. (2002). Principal Component Analysis. Springer. 

Hastie, T., Tibshirani, R., & Friedman, J. (2009). The Elements of Statistical Learning. Springer. 

Kaufman, L., & Rousseeuw, P. J. (2005). Finding Groups in Data: An Introduction to Cluster Analysis. Wiley. 

https://www.kaggle.com/c/imagenet-object-localization-challenge/overview/description

https://www.image-net.org/index.php


