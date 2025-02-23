# Azure Inteligência Artificial(IA) - Serviço Machine Learning Workspace
O objetivo deste laboratório é configurar um modelo de machine learning para desenvolver uma previsão baseada em dados históricos de aluguel de bicicletas.

Ferramentas utilizadas:<br>
    • Azure: https://azure.microsoft.com/pt-br/get-started/azure-portal/<br>
    • Serviço da Azure: Azure Machine Learning<br>
Resumo (Passo-a-passo): Configuração Machine Learning:<br>
    • Selecionar o serviço de IA Machine Learning<br>
    • Escolher a opção "New Workspace" no botão "Create"<br>
    • Preencher os dados solicitados a Aba "Basics"<br>
    • Demais configurações manter o padrão<br>
    • Validar as configuração e criar<br>
    
Detalhamento (Passo-a-passo): Configuração Machine Learning<br>

01 - Selecionar o serviço Azure Machine Learning:<br>
![Image](https://github.com/user-attachments/assets/fb11147a-8716-476f-90ab-29a423df3874)

02 - Clicar no botão "Create" na e na opção "New Workspace": 
![Image](https://github.com/user-attachments/assets/03e2d3f0-2a41-4395-a66b-286c97b2c94d)

03 – Preencher os dados solicitados na Aba “Básicos”:

Detalhes do Workspace:

 * **Nome:** Nome do seu projeto ou modelo. Deve ser único.<br>
 * **Região:** Define em qual servidor da Microsoft você deseja salvar. Essa escolha também pode determinar a moeda que será cobrada pelo uso do serviço.<br>
 * **Conta** de armazenamento: No exemplo, será preenchido automaticamente, pois estamos criando um novo. Basta manter como está. No entanto, caso deseje,<br> 
  pode criar uma estrutura personalizada. Esse armazenamento é utilizado para guardar os artefatos gerados ao rodar o modelo.<br>
 * **Cofre de chaves:** Local onde são armazenados segredos, certificados e informações confidenciais. Para o exemplo, manteremos o que será criado automaticamente,<br> 
  mas no dia a dia, pode-se criar uma estrutura de acordo com as necessidades específicas.<br>
 * **Application Insights:** Ferramenta usada para criação de gráficos e visões, além de monitorar novos valores ou eventos.<br>
 * **Registro de contêiner:** Deve ser mantido como “Nenhum”.<br>
 ![Image](https://github.com/user-attachments/assets/55182448-5b55-4d53-82b5-82a546a3c29d)

04 – Fazer a validação das configurações realizada na Aba ***Examinar + criar*** e em seguida clicar no botão ***criar***.
![Image](https://github.com/user-attachments/assets/76fbb9a6-b255-4471-a49e-08880b272bf9)

Após clicar no botão criar , aguarde o processo ser concluído. 
![Image](https://github.com/user-attachments/assets/5600e2e7-df03-4168-b70a-e0b293f317be)

##Próximo Passo:

01 - Clicar no botão no final da tela: *ir para recurso*
![Image](https://github.com/user-attachments/assets/60f5b024-d670-42cd-9fb4-38ef17efacdf)

02 - Clicar no botão ***Launch studio***
![Image](https://github.com/user-attachments/assets/50d20fff-abce-44bc-bad9-4531fe92f81a)

03 – Abrirá uma nova página, após carregar a página clicar em “ML Automatizado”.
![Image](https://github.com/user-attachments/assets/4fd01a7f-655a-43de-8e7e-78bc2376819b)

04  – Selecionar a item: novo trabalho do ML automatizado.
![Image](https://github.com/user-attachments/assets/bd5ae1cc-123d-4e4b-801d-34a3e7c47a40)

05 – Agora iremos preencher conforme o padrão solicitado, pois estamos executando um exercício disponibilizado pela Microsoft. No entanto, <br>
inclua os dados compatíveis com o modelo que está sendo desenvolvido. Após preencher, clique em **Avançar**.
 * Nome do trabalho: mslearn-bike-automl
 * Nome do experimento: Padrão do sistema, não alterar.
 * Novo nome do experimento: mslearn-bike-rental
 * Descrição: Aprendizado de máquina automatizado para previsão de aluguel de bicicletas
 * Marca: nenhum
![Image](https://github.com/user-attachments/assets/2f7066f8-2684-400a-aef7-3b9a2db4fc9c)


06 – Preencher com os dados *Tipo de tarefa e dados*
  * Selecionar tipo de tarefa: aqui que tipo de tarefa será realizado: uma **regressão**.
![Image](https://github.com/user-attachments/assets/69534f4f-6be4-46c0-86f7-c4061a3f0d22)

07 - Na parte selecionar os dados , clicar no botão Criar . Então, vai abrir uma tela para preencher, após preenchimento clicar em: Avançar
    * Tipo de dados:
      * Nome : aluguel-de-bicicletas
      * Descrição: Dados históricos de aluguel de bicicletas 
      * Tipo: tabular.
![Image](https://github.com/user-attachments/assets/2609a063-893f-48b1-9f04-c2ac9c5b2672)
* Criar ativo de dados: Selecionar a opção De ***arquivos locais*** depois ***Avançar**
  ![Image](https://github.com/user-attachments/assets/ff4fc0be-288a-43d1-89a5-7bd4aa1a5d8e)
 * Nesta tela mantém a configuração padrão em seguida **Avançar**
   * **Tipo de armazenamento de dados:** Azure Blob Storage
   * **Nome: workspaceblobstore**
![Image](https://github.com/user-attachments/assets/3a80489b-a8c9-4e22-aed1-e4a8dee605d9)

08 – Será necessário baixar o arquivo e descompactar. Link do arquivo: https://aka.ms/bike-rentals <br>
     Após baixar e descompactar fazer o carregamento do arquivo e Avançar
![Image](https://github.com/user-attachments/assets/6cb88588-8be8-4425-846d-59ae8e649db1)

9 – Na tela de Configuração manterá conforme a imagem abaixo e clicar em avançar.
![Image](https://github.com/user-attachments/assets/e5782a32-3804-479b-923e-fad6e6e16e87)

10 – Em Esquemas manterá o padrão e clicar em avançar.
![Image](https://github.com/user-attachments/assets/f3541218-9c01-4cfc-bf79-2065b11a55d6)

11 – Agora aparecera a tela de Examinar basta clicar em criar.
![Image](https://github.com/user-attachments/assets/a69fa1a3-b3bd-4aa2-90a4-0205aa27ddc4)

12 – Vai mostrar uma mensagem de sucesso na parte superior, selecionar a opção criado, que você criou nos passos anterior e Avançar.
![Image](https://github.com/user-attachments/assets/357f8673-605e-413d-b042-a8632405a2e8)

13 - Agora neste passo, a configuração necessaria é selecionar Target column: rentals (Integer)
E abaixo do campo acima selecionar e ajustar: View additional configuration settings
![Image](https://github.com/user-attachments/assets/86fba84e-0f9d-4379-8072-4d72e49575d7)
Então, vai abrir uma nova tela onde vai precisar desmarcar as 3 opções:
 * Explicar o melhor modelo
 * Habilitar empilhamento de ensemble
 * usar todos modelos suportados
 * Na opção: Modelos permitidos, selecionar "RandomForest" e "LightGBM"
![Image](https://github.com/user-attachments/assets/6a6f6acc-382f-4cf0-83bf-23c574bb9cac)

14 - Agora, em configuração "Limits", irá configurar o tempo limite, máximo de avaliação entre outras. São os parâmetros para indicar<br>
     o limite e tempo de pesquisas vai ser realizado para apresentar o resultado.
![Image](https://github.com/user-attachments/assets/de754e42-5e23-4838-bfa1-553df8cfe02e)

15 – Em Validar e testar, preencher conforme indicações abaixo e Avançar
    • Tipo de validação: Divisão de validação de treinamento
    • Validação de percentual de dados: 10
    • Dados de teste: Nenhum
![Image](https://github.com/user-attachments/assets/eee87d43-d69d-4379-9e8e-9fc4028086ce)

16 – Agora, selecionar as configurações o desempenho que gostaria para realizar essa tarefa. Vamos manter as configurações padrão e clicar em **avançar**.
![Image](https://github.com/user-attachments/assets/2e1a8705-40a5-401f-b383-92969d4e905a)

Vai apresentar uma tela com resumo das configurações realizadas e clicar em ***Enviar trabalho de treinamento***. 
![Image](https://github.com/user-attachments/assets/624327df-cb83-41bd-8fec-f8fef5786f51)

Não saia da tela. Aguardar concluir:
![Image](https://github.com/user-attachments/assets/17566bde-92db-4864-baf9-c219806e11d3)

Status de concluído:
![Image](https://github.com/user-attachments/assets/99313886-b945-4dc0-aaa3-fd2179c08e63)

02 – Após validação, ir para Modelos e registro, Selecione *“De uma saída do trabalho”*.
![Image](https://github.com/user-attachments/assets/041daacf-4143-426c-b31c-2256e4541819)

03 – O modelo criado selecione o último item e clicar em avançar.
![Image](https://github.com/user-attachments/assets/75acbbca-80b0-415d-b883-4c99d051b215)

04 – O sistema fara a configura automaticamente. Apresenta até uma mensagem informando se ocorreu tudo certo. Mantenha as configurações e vá em avançar.
![Image](https://github.com/user-attachments/assets/b0595fb8-ff0b-40a9-83f6-4a2a6430f942)

05 – Inserir os dados para registrar o modelo e clicar botão ***“Avançar”***:<br>
   *  Nome: bike-rentals.
   *  Descrição: Dados históricos de aluguel de bicicletas..
   *  Versão: Iniciamos com a versão "1".
   *  Marcas: Opcional.
![Image](https://github.com/user-attachments/assets/50cfadf1-f188-42ce-94c0-e224ad978b13)

06 – Na tela examinar e clicar em ***“Registro”**
![Image](https://github.com/user-attachments/assets/a2171656-0a44-49f8-9569-62fba1cdcd5e)

07 - Após registro, volte para o menu "Tarefas" e ir na Aba de "Métricas". O resultado será apresentado.
![Image](https://github.com/user-attachments/assets/5299ff4c-c62a-459e-bc7c-7ef04852c892)

![Image](https://github.com/user-attachments/assets/4941b30f-8ef8-45dd-9de5-62b8df1bbc52)


