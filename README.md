# 📊 Previsão de Estoque Inteligente na AWS com [SageMaker Canvas](https://aws.amazon.com/pt/sagemaker/canvas/)

Este arquivo foi editado para a entrega do projeto "Previsão de Estoque Inteligente na AWS com SageMaker Canvas, sendo esta versão para a entrega e conclusão do Bootcamp.

## 📋 Pré-requisitos

Antes de começar, certifique-se de ter uma conta na AWS. Se precisar de ajuda para criar sua conta, confira nosso repositório [AWS Cloud Quickstart](https://github.com/digitalinnovationone/aws-cloud-quickstart).


## 🎯 Objetivos Deste Desafio de Projeto (Lab)

![image](https://github.com/digitalinnovationone/lab-aws-sagemaker-canvas-estoque/assets/730492/72f5c21f-5562-491e-aa42-2885a3184650)

:heavy_check_mark: Dê um fork neste projeto e reescreva este `README.md`. Sinta-se à vontade para detalhar todo o processo de criação do seu Modelo de ML para uma "Previsão de Estoque Inteligente".

:heavy_check_mark: Para isso, siga o [passo a passo] descrito a seguir e evolua as suas habilidades em ML no-code com o Amazon SageMaker Canvas.

:heavy_check_mark: Ao concluir, envie a URL do seu repositório com a solução na plataforma da DIO.


## 🚀 Passo a Passo

### 1. Selecionar Dataset

:heavy_check_mark:Navegue até a pasta `datasets` deste repositório. Esta pasta contém os datasets que você poderá escolher para treinar e testar seu modelo de ML. Sinta-se à vontade para gerar/enriquecer seus próprios datasets, quanto mais você se engajar, mais relevante esse projeto será em seu portfólio.

:heavy_check_mark:   Escolha o dataset que você usará para treinar seu modelo de previsão de estoque.

:heavy_check_mark:   Faça o upload do dataset no SageMaker Canvas.

**-  :heavy_exclamation_mark:  O dataset escolhido para a tarefa foi o "dataset-1000-com-preco-promocional-e-renovacao-estoque.csv".**

### 2. Construir/Treinar

:heavy_check_mark:   No SageMaker Canvas, importe o dataset que você selecionou.

:heavy_check_mark:   Configure as variáveis de entrada e saída de acordo com os dados.

:heavy_check_mark:   Inicie o treinamento do modelo. Isso pode levar algum tempo, dependendo do tamanho do dataset.

**-    :heavy_exclamation_mark: A variável escolhida para ser prevista foi a QUANTIDADE_ESTOQUE e a variável temporal foi a "DATA_EVENTO", com previsão para 9 dias.**

### 3. Analisar

:heavy_check_mark:   Após o treinamento, examine as métricas de performance do modelo.

:heavy_check_mark:   Verifique as principais características que influenciam as previsões.

:heavy_check_mark:   Faça ajustes no modelo se necessário e re-treine até obter um desempenho satisfatório.

**-    :heavy_exclamation_mark: Após o treinamento, observou-se que as variáveis "PRECO" e "FLAG_PROMOCAO", que representam, respectivamente, o preço dos produtos e se houveram promoções, tem uma correlação variável com a "QUANTIDADE_ESTOQUE"; tendo um impacto de apenas 35,29% para a primeira variável e 0% para a segunda. Sendo assim, é possível concluir que "PRECO" têm alguma influência em "QUANTIDADE_ESTOQUE", enquanto que "FLAG PROMOCAO" não influencia em nada**

### 4. Prever

:heavy_check_mark:   Use o modelo treinado para fazer previsões de estoque.

:heavy_check_mark:   Exporte os resultados e analise as previsões geradas.

:heavy_check_mark:   Documente suas conclusões e qualquer insight obtido a partir das previsões.

**-    :heavy_exclamation_mark: Com o treinamento, foram geradas previsões para todos os produtos, onde foi gerado o arquivo "XXXXX", upado nesse fork. Mas para exemplificar um resultado, utilizamos a previsão do produto XXXXXX, ilustrado na imagem abaixo.**

![image](https://github.com/digitalinnovationone/lab-aws-sagemaker-canvas-estoque/assets/730492/72f5c21f-5562-491e-aa42-2885a3184650)

**-   :heavy_exclamation_mark: Como podemos ver, para as 3 previsões, (padrão otimista e pessimista), foi previsto um XXXX do estoque, indicando uma alta demanda do produto e talves sendo necessário suprir o estoque**

**-  :heavy_exclamation_mark: As métricas encontradas do modelo foram:**

    ## ABLA: 
    
    ## BABLA:
    
    ## Cabla:
    
    ## 

## 🤔 Dúvidas?

Esperamos que esta experiência tenha sido enriquecedora e que você tenha aprendido mais sobre Machine Learning aplicado a problemas reais. Se tiver alguma dúvida, não hesite em abrir uma issue neste repositório ou entrar em contato com a equipe da DIO.
