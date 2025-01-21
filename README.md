# Azure Inteligência Artificial(IA) - Visão Computacional: Configuração do Resource
Criar repositorio onde será salvo o projeto juntamente configurar AI Vision Service e realizar testes práticos.


### Ferramentas utilizadas:

- Portal Azure: https://portal.azure.com/#home
- Portal Studio Vision : https://portal.vision.cognitive.azure.com/

### Pontos Importantes:

- Caso esteja realizando apenas um prática de estudo, no final excluir tudo que foi construído nesse laboratório. Desta forma, minimiza o risco de ser cobrado algum valor. Lembre-se você está em um ambiente real de produção.
- Documentação:
    + https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/03-image-analysis.html
    + https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/04-face.html
    + https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/05-ocr.html

### Resumo (Passo-a-passo): Configuração Vision Service:

- Entrar no ambiente Azure
- Criar o resource onde será salvo o projeto
- Entrar no Studio IA
- Definir o resource como Default

### Detalhamento (Passo-a-passo): Configuração Vision Service

01 - Criar o serviço que iremos utlizar confirme link abaixo:

https://github.com/WanderBernardo/AzureIA_ServiceAzureAIservices

### Após concluir a as configurações acima, Entrar no portal: ``` https://portal.vision.cognitive.azure.com/ ```

Esse portal é o Studio onde vamos trabalhar com a Inteligência Artificial (IA)

05 - Após realizar o login no site do Studio, então selecionar o resource criado na configuração acima. Clicar para visualizar todos resources.
![image](https://github.com/user-attachments/assets/f8221fac-044a-46a9-9282-3f6ff24a9294)

06 - Agora, selecionar o resource criado e clicar no botão ``` Select as default resource ```. Se tiver tudo certo, não vai acontecer nada. A tela não vai tremer! ksksk. Então click no botão ``` X ``` para voltar a tela anterior.
![image](https://github.com/user-attachments/assets/895c1d5f-d79e-446c-abb6-c5ae3273d704)

### Atenção

Caso esse ultimo passo apresente erro: ResourceOperationFailure: Resource provider [N/A] isn't registered with Subscription [N/A] . Então, deve realizar uma configuração e refazer a confiuração acima.
   * Ir no portal da Azure: https://portal.azure.com/#home, fazer o login
   * Na barra de pesquisa, escrever "Subscription"
   * Selecionar o Subscription Name
   * Vai abrir um novo menu, então selecionar "Resource providers"
   * Selecionar:
      + Microsoft.Cdn
      + Microsoft.CostManagement
   * Clicar no botão acima "Register".

   ![image](https://github.com/user-attachments/assets/79e279f1-96a9-4301-978a-71128c464908)

Links de ajuda:
   * https://learn.microsoft.com/en-us/answers/questions/1983847/error-while-creating-a-managed-online-endpoint-in
   * https://learn.microsoft.com/en-us/answers/questions/2129910/resource-provider-(n-a)-isnt-registered-with-subsc

### Próximo Passo

https://github.com/WanderBernardo/AzureIA_ComputerVision_ServicesTests

