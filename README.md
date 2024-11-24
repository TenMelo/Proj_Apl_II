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

## 1.3  Comparativo evolutivo dos algoritmos ao longo dos anos 
A evolução da geração de imagens com inteligência artificial tem tido saltos astronômicos 
de qualidade, alinhando resultados com praticidades essa tecnologia tem impactado 
positivamente todos os mercados de publicidade, entretenimento e quaisquer outros que 
necessitem de elementos visuais como suporte para a expressão de sua mensagem. Nesse 
contexto nosso projeto se apresenta como uma solução extremamente pertinente para esse 
crescente mercado em evolução. 

Um exemplo de tal pode ser visto na seguinte imagem que ilustra a evolução da tecnologia 
no passar dos anos

![Captura de tela 2024-11-23 211816](https://github.com/user-attachments/assets/dc18025f-b281-43de-83c6-c9e14681b77f)

## 1.4 DEFINIÇÃO DAS LINGUAGENS UTILIZADAS
Neste projeto será utilizada a linguagem Python por se tratar de uma linguagem amplamente usada no meio da ciência da computação para aprendizado de máquina, projetos que envolvem Deep Learning, entre outros exemplos, o que além a tornarem uma ferramenta eficaz, faz com existam diversos repositórios de código que contribuem para o desenvolvimento de outros projetos.

## 1.5 BASE DE DADOS
A base de dados utilizada será uma base do site ImageNet, também disponível no Kaggle, ofertada pela Princeton University e Stanford University, que se trata de uma série de imagens rotuladas que servirão tanto para o treinamento do modelo que irá entender a imagem através de visão computacional, para que assim possa decodificá-la, quanto para a possível geração de imagens melhores que as fornecidas pelo MidJourney, pelos parâmetros elaborados anteriormente.

## 1.6 CRONOGRAMA

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
## 2.3 MÉTODO ANALÍTICO 

A fim de reduzir o escopo do problema para torná-lo de mais simples resolução, iremos focar no quesito da problemática da geração de textos compreensíveis e coesos em imagens geradas artificialmente. Nesse caso, iremos trabalhar com a ideia de IAs colaborativas, onde temos dois sistemas que trabalham com um mesmo objetivo, complementando seu desenvolvimento. 

Para tanto, a IA generativa será responsável pela geração de alguma imagem que contenha um texto fornecido no seu prompt, enquanto a IA possuidora do Optical Character Recognition (OCR) deverá identificar o texto, comparar com a informação dada no prompt e, por fim, seu resultado deverá servir como feedback para correção do 1º sistema, incentivando a criação de imagens com textos reais. De forma resumida, organizaremos o algoritmo em três etapas conforme segue: 

Etapa 1: Geração da imagem com texto no prompt; 

Etapa 2: Identificação do texto do texto via algoritmo de OCR e comparação com o texto do prompt; e 

Etapa 3: Correção do texto se necessário e feedback da informação de erro. 

## 2.4 DEFINIÇÃO E DESCRIÇÃO DA ACURÁCIA 
A acurácia será calculada através de um método simples de verificação pela comparação citada anteriormente, entre o texto fornecido no prompt da geração de imagens e o resultado obtido pela IA detentora de OCR, ferramenta consolidada desenvolvida para leitura de textos em imagens, que deverá identificar se há algo escrito na imagem e comparar a semântica com a do comando, onde será por fim calculada a acurácia pela taxa de correspondência entre os caracteres gerados e lidos com os do anteriormente mencionado prompt. 

## 2.5 RESULTADOS PRELIMINARES 
Concretizando os objetivos apresentados anteriormente, esta etapa servirá como um proof of concept, ou uma prova de conceito, de que através do uso de IAs colaborativas é possível melhorar aspectos individuais da geração de imagem, no caso, o texto apresentando se tornando cada vez mais real e conciso, de aplicação prática em um contexto de mundo real. 

Evidencia-se, assim, que ao corrigir erro tão crasso nos sistemas atuais, exploraremos uma oportunidade de mercado muito forte, haja vista que muitas pessoas e empresas necessitam hoje de um complemento às suas gerações de imagem quando falamos de elementos textuais, sendo necessário a contratação de um designer, por exemplo, para cobrir essas áreas atualmente fora do domínio das IAs generativas. Sanando este problema, teremos uma fatia de mercado exponente que estará ávida pelas novas soluções em Inteligência Artificial. Como exemplo da aplicação segue alguns exemplos teóricos da aplicação do script descrito: 

![imagem 1](https://github.com/user-attachments/assets/5d719aad-3c29-4ec1-bae3-3218bec1b542)

Imagem 1: Identificação e correção do texto ”Happy Birthday” 

![image 2](https://github.com/user-attachments/assets/86e8db82-ebc1-4540-bb53-3050bd8cbf17)

Imagem 2: Identificação e correção do texto ”CADERE IN PIEDI COME I GATTI” 

![image 3](https://github.com/user-attachments/assets/fc5acaf3-290e-41b0-823a-7bb3c507b2a0)

Imagem 3: Identificação e correção do texto  ”Clothing Store” 

 

# 3. STORYTELLING 

Inicialmente o trabalho buscava apresentar os conceitos da geração de imagens em modelos de IA generativa e apresentar melhores técnicas de prompt visando a melhor geração de imagens, porém devido a imprevistos como o alto nível de complexidade encontrados, optou-se por reduzir o escopo para otimização da geração de imagens em pontos-chave como a geração de textos em imagens, se utilizando da visão computacional.  

O tema se mostra cada vez mais relevante no contexto da economia de atenção, em que o usuário está constantemente bombardeado por inúmeros estímulos diferentes como vídeos rápidos no TikTok, streamings, entre outros, sendo necessário uma agilidade quase que sobre humana dos times de desenvolvimento para competir e poder captar a atenção do usuário para si. 

Nesse contexto o projeto visa utilizar as novas tecnologias de IA e suas técnicas de processamento de linguagem natural para traduzir as ideias de desenvolvimento em entradas do algoritmo para enfim obter o resultado esperado em tempo recorde com uma maior precisão. 

O estudo do projeto visa desvendar qual a melhor combinação de caracteres e seus impactos na geração de imagens para a visão computacional, explicando de forma superficial os processos de codificação do prompt, stemming (Derivação), análise de dependência e a decodificação. 

A codificação do prompt é o processo de transformação da entrada em bits para que o algoritmo possa entender o que cada palavra isoladamente significa, posteriormente o stemming ou Derivação, pegará todo o prompt decodificado e analisará o resultado do processo anterior para desvendar o sentido completo de cada frase, assim posteriormente na fase de análise de dependência o programa passará a entender como as frases se relacionam a fim de entender o sentido completo de todo o prompt para, então, na fase de decodificação ser executada a ordem e decodificado o resultado. 

Para medirmos a acurácia e o grau de perda de informação optamos por confrontar a imagem gerada pela primeira IA com um algoritmo de OCR (Optical Character Recognition) que será responsável por ler o texto da imagem, possibilitando a automação do processo do cálculo de acurácia via pesquisa do texto lido em um dicionário, revelando se é de fato uma palavra ou frase existente. 

No mais, o trabalho se mostra extremamente relevante para o cenário atual de competição acirrada pela atenção das pessoas, agregando dinamicidade, variedade e assertividade para a criação de conteúdo e atendimento das expectativas dos stakeholders. 
 
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


