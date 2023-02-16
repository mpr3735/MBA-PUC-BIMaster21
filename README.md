<!-- antes de enviar a versão final, solicitamos que todos os comentários, colocados para orientação ao aluno, sejam removidos do arquivo -->
# Classificação de Imagens com Transfer Learning

#### Aluno: [Mauricio Pereira Rangel](https://github.com/link_do_github)
#### Orientador: [Felipe Borges](https://github.com/FelipeBorgesC) e [Nome Sobrenome](https://github.com/link_do_github).
#### Co-orientador(/a/es/as): [Nome Sobrenome](https://github.com/link_do_github) e [Nome Sobrenome](https://github.com/link_do_github). <!-- caso não aplicável, remover esta linha -->

---

Trabalho apresentado ao curso [BI MASTER](https://ica.puc-rio.ai/bi-master) como pré-requisito para conclusão de curso e obtenção de crédito na disciplina "Projetos de Sistemas Inteligentes de Apoio à Decisão".

<!-- para os links a seguir, caso os arquivos estejam no mesmo repositório que este README, não há necessidade de incluir o link completo: basta incluir o nome do arquivo, com extensão, que o GitHub completa o link corretamente -->
- [Link para o código](https://github.com/link_do_repositorio). <!-- caso não aplicável, remover esta linha -->

- [Link para a monografia](https://link_da_monografia.com). <!-- caso não aplicável, remover esta linha -->

- Trabalhos relacionados: <!-- caso não aplicável, remover estas linhas -->
    - [Nome do Trabalho 1](https://link_do_trabalho.com).
    - [Nome do Trabalho 2](https://link_do_trabalho.com).

---

### Resumo

<!-- trocar o texto abaixo pelo resumo do trabalho, em português -->

O presente estudo tem como escopo a análise comparativa da aplicação do conceito da técnica de transfer learning, em classificação de imagens, de quatro modelos de redes CNN. O objetivo é utilizar uma estrutura padrão de camadas em cada uma das redes CNN, em análise, e alterar um conjunto de parâmetros determinados, para avaliar o impacto dos mesmos no resultado de cada execução, de cada modelo de rede CNN. Com isso identificar se há relevância ou não, em cada uma dessas variações nos resultados coletados das execuções dos modelos, considerando um corte ideal para os valores das métricas de predição. Não faz parte do escopo atingir o máximo de performance no resultado de cada modelo.

### Abstract <!-- Opcional! Caso não aplicável, remover esta seção -->

<!-- trocar o texto abaixo pelo resumo do trabalho, em inglês -->

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Proin pulvinar nisl vestibulum tortor fringilla, eget imperdiet neque condimentum. Proin vitae augue in nulla vehicula porttitor sit amet quis sapien. Nam rutrum mollis ligula, et semper justo maximus accumsan. Integer scelerisque egestas arcu, ac laoreet odio aliquet at. Sed sed bibendum dolor. Vestibulum commodo sodales erat, ut placerat nulla vulputate eu. In hac habitasse platea dictumst. Cras interdum bibendum sapien a vehicula.

Proin feugiat nulla sem. Phasellus consequat tellus a ex aliquet, quis convallis turpis blandit. Quisque auctor condimentum justo vitae pulvinar. Donec in dictum purus. Vivamus vitae aliquam ligula, at suscipit ipsum. Quisque in dolor auctor tortor facilisis maximus. Donec dapibus leo sed tincidunt aliquam.

Donec molestie, ante quis tempus consequat, mauris ante fringilla elit, euismod hendrerit leo erat et felis. Mauris faucibus odio est, non sagittis urna maximus ut. Suspendisse blandit ligula pellentesque tincidunt malesuada. Sed at ornare ligula, et aliquam dui. Cras a lectus id turpis accumsan pellentesque ut eget metus. Pellentesque rhoncus pellentesque est et viverra. Pellentesque non risus velit. Orci varius natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus.

### 1. Introdução

A base de dados para a realização do estudo analítico comparativo foi obtida do kaggle e contém 38 classes de tipos de plantas saudáveis ou com algum tipo de doença (fungo). Foi realizada uma análise da quantidade de ocorrências de imagens, em cada classe, e para adapta;'ao a limites do ambiente de execução (processamento e consumo de GPU) foi necessário um corte reduzindo o escopo para 04 classes da categoria Uva, o que não afeta o objetivo do estudo. O processo para utiliizar a t[ecnica de transfer learming adotou a base de imagens da Imaginet e principalmente consultas em exemplos do Keras (keras.org), nesse contexto.  Ap[os a an[alise e preparo da base de dados de imagens foram elaborados quatro notebooks python, um para cada rede CNN com transfer learning e realizadas oito execu;'oes de cen[arios dos modelos, conservando uma estrutura commum de camadas e neur"onios e variando determinados par'metros comuns, para coleta e compara;'ao dos valores das m[etricas de treino , vaida;'ao e testes.

### 2. Modelagem

O modelo proposto para a an[alise comparativa das redes CNN com transfer learning foi estabelecido da seguinte forma?
Utilizar uma Base de dados de entrada com 04 classes de imagens de doen;as em folhas de Uvas (xxxx, xxxx, xxxx, xxxxx). A classe xxx foi descartada ap[os an[alise da quantidade de imagens, na etapa de an[alise das frequ"encias de imagens em cada classe. Constru;'ao de quatro c[odigos em python, padronizados, com utiliza;'ao de tranfer learning, uso da Imaginet, e com base nos modelos CNN Resnet50, Xception, VGG19 e VGG16. Para que a an[alise comparativa ficasse preservada foi utilizada a mesma estrutura da camada dense e quantidade de neuronios, para cada modelo de rede CNN (Dense1xxx, Dense2.....). Com base nesse padrao, condi;'oes e restri;'oes foram executados oito cena[rios, para cada modelo de rede CNN, com varia;'ao em combina;'oes dos par"ametros Early Rate, Early Stop, Dropout e BatchNormalization. O modelo n'ao considerou a utiliza;'ao da t[ecncia de dataaugmentation , por estar fora do escopo.

A codifica;'ao de notebooks python, para cada modelo CNN adotou um padr'ao, com as seguintes etapas? Defini;'ao dos dados de treino, valida;'ao e testes. Contagens de cada classe e quantidade de imagens nas mesmas. Preparo de cada conjunto de dados de treino, valida;'ao e teste, com an[alise do shape das imagens e normaliza;'ao dos dados de entrada. Ana[lise da estrutura da rede CNN em quest'ao. An[alise da estrutura da rede CNN truncada. An[alise das camadas do modelo final com transfer learning e camdas Dense. Compila;'ao do modelo. Treino e An[alise das m[etricas. Testes e Infer"encia.

Com esse padr'ao de codifica;a'o facilitou a execu;'ao recrusiva dos modelos e coleta das informa;'eos nos oito cen[arios. Sendo o oitavo cen[ario o ponto de corte para a an[lise comparativa final.





d) Mesma Estrutura da camada dense para cada modelo (
e) Execu;'ao de oito cen[arios de cada rede CNN, citada, considerando treino, valida;'ao e testes, com coleta das m[etricas de xxxxxxxxxxxx
e.1) Para cada cen[ario uma defini;'ao de combina;'ao de valores e ativa;'oes dos par"ametros elarly rate, early stop, dropout e batchnormalization.
f)An[alise e compara;'ao dos resultados dos valores coletados


Lorem ipsum dolor sit amet, consectetur adipiscing elit. Proin pulvinar nisl vestibulum tortor fringilla, eget imperdiet neque condimentum. Proin vitae augue in nulla vehicula porttitor sit amet quis sapien. Nam rutrum mollis ligula, et semper justo maximus accumsan. Integer scelerisque egestas arcu, ac laoreet odio aliquet at. Sed sed bibendum dolor. Vestibulum commodo sodales erat, ut placerat nulla vulputate eu. In hac habitasse platea dictumst. Cras interdum bibendum sapien a vehicula.

Proin feugiat nulla sem. Phasellus consequat tellus a ex aliquet, quis convallis turpis blandit. Quisque auctor condimentum justo vitae pulvinar. Donec in dictum purus. Vivamus vitae aliquam ligula, at suscipit ipsum. Quisque in dolor auctor tortor facilisis maximus. Donec dapibus leo sed tincidunt aliquam.

### 3. Resultados

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Proin pulvinar nisl vestibulum tortor fringilla, eget imperdiet neque condimentum. Proin vitae augue in nulla vehicula porttitor sit amet quis sapien. Nam rutrum mollis ligula, et semper justo maximus accumsan. Integer scelerisque egestas arcu, ac laoreet odio aliquet at. Sed sed bibendum dolor. Vestibulum commodo sodales erat, ut placerat nulla vulputate eu. In hac habitasse platea dictumst. Cras interdum bibendum sapien a vehicula.

Proin feugiat nulla sem. Phasellus consequat tellus a ex aliquet, quis convallis turpis blandit. Quisque auctor condimentum justo vitae pulvinar. Donec in dictum purus. Vivamus vitae aliquam ligula, at suscipit ipsum. Quisque in dolor auctor tortor facilisis maximus. Donec dapibus leo sed tincidunt aliquam.

### 4. Conclusões

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Proin pulvinar nisl vestibulum tortor fringilla, eget imperdiet neque condimentum. Proin vitae augue in nulla vehicula porttitor sit amet quis sapien. Nam rutrum mollis ligula, et semper justo maximus accumsan. Integer scelerisque egestas arcu, ac laoreet odio aliquet at. Sed sed bibendum dolor. Vestibulum commodo sodales erat, ut placerat nulla vulputate eu. In hac habitasse platea dictumst. Cras interdum bibendum sapien a vehicula.

Proin feugiat nulla sem. Phasellus consequat tellus a ex aliquet, quis convallis turpis blandit. Quisque auctor condimentum justo vitae pulvinar. Donec in dictum purus. Vivamus vitae aliquam ligula, at suscipit ipsum. Quisque in dolor auctor tortor facilisis maximus. Donec dapibus leo sed tincidunt aliquam.

---

Matrícula: 123.456.789

Pontifícia Universidade Católica do Rio de Janeiro

Curso de Pós Graduação *Business Intelligence Master*
