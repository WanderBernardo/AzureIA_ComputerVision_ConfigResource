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

01 - Após logar no portal Azure. Criar um ``` Create a resource  ```
![image](https://github.com/user-attachments/assets/74e81e19-8c4d-42db-a3c6-9b93d4fe95bb)

02 - Na barra de pesquisa digitar a opção: ``` Azure AI services  ```. Cuidado que no meu caso apresentou duas opções com o mesmo nome, mas vão usar a opção que tem o ícone de nuvem.
![image](https://github.com/user-attachments/assets/8b61c68c-e269-4090-8d8b-b44b5d761077)

Clicar em botão: ``` Create ```
![image](https://github.com/user-attachments/assets/e658a628-f329-412f-a30f-4a9474610872)

03 - Iniciar a configuração criando o repositório onde será salvo nosso projeto, modelo, laboratório. Fique a vontade para chamar do melhor padrão para sua necessidade.
   * Subscription: é a conta que você está logado. É como se você a sua empresa. Repositótorio geral de tudo que é criado, a Pasta principal. Já vem preenchido de padrão, Esse padrão é criado automaticamente quando realiza o cadastro. Mas pode ser criado outras opções.
   * Resource group: é uma sub-repositório do "Subscription".
Imagina uma gaveteiro onde o gaveteiro inteiro é Subscriptiom e uma gaveta desse gaveteiro é o Resource group.
   * Region: basicamente, quer dizer em qual servidor da Microsoft você quer salvar(brasil, USA etc). Acredito que também determina a moeda que será cobrado por utilizar esse serviço.
   * Name: nome do seu projeto, modelo (Deve ser único)
   * Pricing tier: Selecionar a padrão do sistema.
   * Check box: "By checking this box I acknowledge that I have read and understood all the terms below". Deve marcar, pois precisa aceitar os termos e condições.
![image](https://github.com/user-attachments/assets/188b515a-fd4e-4973-9983-d3505ae796ad)

04 - Demais Abas: vamos manter o padrão, pois estamos realizando uma configuração basica e iremos excluir esse modelo no final. Então, click no botão ``` Review + create ``` para validar as configurações e depois click novamente no botão ``` Create ``` 
   * Networking: configuração de privacidade do seu modelo(Publico/Privado)
   * Identity: usar o controle de acesso
   * Tags: muito usado para criar filtros. Por exemplo: Quero fazer rateio para lançamento de custo por Departamento, então, cria as tags por departamento. Conforme sua necessidade.
![image](https://github.com/user-attachments/assets/8c6870b4-9686-4c93-b5c8-a049315f8e6b)

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
