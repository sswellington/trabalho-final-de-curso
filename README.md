# Trabalho Final de Curso :mortar_board:
## Combinando abordagens supervisionadas e não supervisionadas para segmentação de imagens de úlceras em membros inferiores
* [Monografia :memo:](https://github.com/sswellington/trabalho-final-de-curso/blob/master/monografia-min.pdf)
* [Apresentação :man_teacher:](https://github.com/sswellington/trabalho-final-de-curso/blob/master/apresentation.pdf)

## 2019 IEEE 32nd International Symposium on Computer-Based Medical Systems (CBMS)
* [Apresentação :man_teacher:](https://github.com/sswellington/trabalho-final-de-curso/blob/master/apresentation.pdf)
* DOI: [10.1109/CBMS.2019.00076](https://ieeexplore.ieee.org/document/8787493/)

---

## Resumo

A segmentação de tecidos de fotografias de úlceras crônicas em membros inferiores é uma abordagem não intrusiva para análises dermatológicas. 

Este trabalho envolve o estudo e implementação de técnicas de processamento digital de imagens aplicadas à imagens de úlceras em membros inferiores, com o objetivo de segmentar e identificar as diversas classes de tecidos existentes nesse tipo de lesão. 

Para esse propósito foram desenvolvidas uma solução ad-hoc e uma solução baseada em aprendizado de máquina. 

Essa última, denominada 2PLA, é um método que combina estratégias de aprendizado supervisionado e não supervisionado para melhorar a segmentação das imagens dermatológicas. 

Dada uma foto de úlcera capturada de acordo com um protocolo médico fixo, a primeira fase do sistema realiza uma classificação
de pontos de interesse, enquanto filtros de pré-processamento são empregados para suavizar o ruído da imagem. 

A imagem limpa é enviada posteriormente para uma segunda fase que consiste em divisão e conquista, baseada em um algoritmo de construção de superpixels. 

O método 2PLA divide membro inferior em regiões de interesse com bordas bem definida e agrupa os superpixels utilizando o algoritmo DBSCAN, que é baseado em similaridade. 

As duas fases do 2PLA foram avaliadas em um conjunto real de feridas dermatológicas. 

Avaliações empíricas em amostras representativas de até 100.000 pontos mostram que uma rede neural artificial
Perceptron Multi-Layer com o algoritmo de treinamento Levenberg-Marquardt (Coeficiente de Kappa-Cohen = 0,971, Sensibilidade = 0,98 e Especificidade = 0,98) supera outros classifi cadores como a primeira fase da 2PLA. 

Além disso, ensaios experimentais com o DBSCAN e cinco funções de distância (L1 , L2 , L∞ , Canberra e BrayCurtis) indicam que a função L1 gera
menos grupos em comparação a outras funções, percebendo-se um decaimento exponencial da quantidade de grupos em função da taxa de similaridade. O critério do “cotovelo” foi empregado para encontrar o limite do DBSCAN com a função L1 como parametrização da segunda fase do sistema. 

A avaliação final do 2PLA com as duas fases devidamente configuradas em um conjunto rotulado de imagens de úlcera indica que os tecidos foram corretamente segmentados dentro de uma razão de erro absoluto médio de 0,05, o que ilustra o impacto de eficácia do método 2PLA para a segmentação de feridas.

### Notícia
* Aluno Wellington de Souza Silva (Curso de Computação) INFES/UFF e pesquisadores do Grupo ANOTi têm trabalho reconhecido em conferência internacional.[ :link:](http://infes.uff.br/aluno-do-infes-uff-e-pesquisadores-do-grupo-anoti-tem-trabalho-reconhecido-em-conferencia-internacional-aluno-wellington-de-souza-silva-do-curso-de-computacao-do-infes-uff-foi-premiado-como-finalist/)
* A Two-Phase Learning Approach for the Segmentation of Dermatological Wounds[ :link:](https://www.computer.org/csdl/proceedings-article/cbms/2019/228600a343/1cdO0qLxGvK)
* Artigos de pesquisadores do ICMC-USP são premiados em conferência internacional[ :link:](https://www.computer.org/csdl/proceedings-article/cbms/2019/228600a343/1cdO0qLxGvK)
* Computação e medicina: artigos do ICMC são premiados em conferência internacional[ :link:](https://icmc.usp.br/noticias/4404-computacao-e-medicina-artigos-do-icmc-sao-premiados-em-conferencia-internacional)
* Professor do IFNMG é um dos autores de estudo premiado em uma das principais conferências na área de computação, medicina e bioinformática[ :link:](https://www.ifnmg.edu.br/mais-noticias-portal/492-portal-noticias-2019/21351-professor-do-ifnmg-e-um-dos-autores-de-estudo-premiado-em-uma-das-principais-conferencias-na-area-de-computacao-medicina-e-bioinformatica)

### Código Fonte :man_technologist:
> [`2PLA`](https://github.com/sswellington/2PLA)

### Template[ :link:](https://github.com/sswellington/Template_TCC/tree/master/Template)

> Conforme ABNT 

#### Estrutura do TCC

##### 1. Pré-Texto
* Capa 
* Folha de rosto
* Dedicatória (opcional) 
* Agradecimento (opcional)
* Epígrafe (opcional)
* Resumo
* Abstract
* Lista
  * Ilustrações
  * Tabelas
  * Abreviaturas e siglas
  * Símbolos
* Sumário

##### 2. Texto
* Introdução 
	* Motivação e contexto
	* Objetivo
	* Organização da monografia
* Conceito preliminares e levantamento bibligráfico
	* Trabalho relacionado 
	* Conclusão parcial
* Material e método
	* Conclusão parcial
* Experimento e resultado
* Conclusão
	* Dificuldade encontrada
	* Publicação
	* Premiação
	* Trabalho futuro

##### 3. Pós-Textuais
* Referência
* Anexo (opcional)


--- 

## Repercussão do trabalho 
* [UFF-INFES](http://infes.uff.br/aluno-do-infes-uff-e-pesquisadores-do-grupo-anoti-tem-trabalho-reconhecido-em-conferencia-internacional-aluno-wellington-de-souza-silva-do-curso-de-computacao-do-infes-uff-foi-premiado-como-finalist/)
* [ICMC-USP](https://icmc.usp.br/noticias/4404-computacao-e-medicina-artigos-do-icmc-sao-premiados-em-conferencia-internacional)
* [FAPESP](https://agencia.fapesp.br/artigos-de-pesquisadores-do-icmc-usp-sao-premiados-em-conferencia-internacional/31134/)
* [IFNMG](https://www.ifnmg.edu.br/mais-noticias-portal/492-portal-noticias-2019/21351-professor-do-ifnmg-e-um-dos-autores-de-estudo-premiado-em-uma-das-principais-conferencias-na-area-de-computacao-medicina-e-bioinformatica)
* [Computer](https://www.computer.org/csdl/proceedings-article/cbms/2019/228600a343/1cdO0qLxGvK)