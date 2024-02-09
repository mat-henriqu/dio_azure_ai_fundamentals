# dio_azure_ai_fundamentals

# <span style="color:blue">Microsoft Car Sales</span>

## <span style="color:green">Criar uma Plataforma de Vendas no Azure para Automóveis</span>

<span style="color:orange">Utilize o aprendizado automático para prever as preferências do cliente</span>  
<span style="color:orange">Analise o melhor modelo de vendas</span>  
<span style="color:orange">Implante e teste o modelo de vendas</span>  
<span style="color:orange">Teste o serviço de vendas implantado</span>  
<span style="color:orange">Limpeza</span>

Explore o Aprendizado Automatizado de Vendas no Azure Machine Learning  
Neste exercício, você usará o recurso de aprendizado de máquina automatizado no Azure Machine Learning para prever as preferências do cliente e otimizar as vendas de automóveis. Você irá então implantar e testar o modelo de vendas treinado.

Este exercício deve levar aproximadamente 30 minutos para completar.

## <span style="color:green">Criar uma Plataforma de Vendas no Azure para Automóveis</span>

Para usar o Azure Machine Learning, você precisa configurar uma plataforma de vendas no Azure. Siga as etapas abaixo para criar a plataforma:

1. Faça login no [Portal do Azure](https://portal.azure.com) usando suas credenciais da Microsoft.
   
2. Selecione **+ Criar um recurso**, procure por **Vendas de Automóveis** e crie uma nova plataforma de vendas de automóveis no Azure com as seguintes configurações:
   - Assinatura: Sua assinatura do Azure.
   - Grupo de recursos: Crie ou selecione um grupo de recursos.
   - Nome: Insira um nome exclusivo para sua plataforma.
   - Região: Selecione a região geográfica mais próxima.
   - Armazenamento de Dados: Observe a nova conta de armazenamento padrão que será criada para sua plataforma.
   - Segurança: Observe a nova segurança padrão que será configurada para sua plataforma.
   - Insights: Observe o recurso padrão de novos insights que será criado para sua plataforma.
   
3. Selecione **Revisar + Criar** e, em seguida, selecione **Criar**. Aguarde a criação da plataforma (pode demorar alguns minutos) e, em seguida, acesse o recurso implantado.

4. Selecione **Painel de Controle** (ou abra uma nova guia do navegador e navegue até [https://sales.azure.com](https://sales.azure.com), e entre na plataforma de vendas usando sua conta da Microsoft). Feche todas as mensagens que são exibidas.

## <span style="color:green">Utilize o aprendizado automático para prever as preferências do cliente</span>

O aprendizado automático permite prever as preferências do cliente e otimizar as vendas. Siga as etapas abaixo para criar um modelo de vendas:

1. No Painel de Controle da Plataforma de Vendas no Azure, vá para a página de **Aprendizado Automático** (abaixo de **Autorização**).

2. Crie um novo projeto de aprendizado automático com as seguintes configurações:
   - **Configurações básicas**:
     - Nome do projeto: mslearn-car-sales-automl
     - Novo nome do experimento: mslearn-car-sales-prediction
     - Descrição: Previsão de preferências do cliente para vendas de automóveis
     - Tags: Nenhuma
   - **Tipo de tarefa e dados**:
     - Selecione o tipo de tarefa: Classificação
     - Selecione o conjunto de dados: Crie um novo conjunto de dados com as seguintes configurações:
       - Tipo de dados: Tabular
       - Nome: Preferências do Cliente
       - Descrição: Dados históricos de preferências do cliente
       - Fonte de dados: Selecione De arquivos web
       - URL da Web: Insira a URL do seu conjunto de dados de preferências do cliente
       - Ignorar a validação de dados: Não selecione
       - Configurações: Defina o formato de arquivo, delimitador, codificação e cabeçalhos de coluna conforme necessário
       - Esquema: Revise e ajuste os tipos de dados conforme necessário
     - **Configurações da tarefa**: Especifique a coluna alvo e outras configurações relacionadas à tarefa de classificação.
   - **Configurações de computação**: Especifique as configurações de computação para treinamento do modelo.

3. Envie o projeto de aprendizado automático. O treinamento do modelo começará automaticamente.

4. Aguarde o treinamento do modelo ser concluído. Isso pode levar algum tempo, então seja paciente.

## <span style="color:green">Analise o Melhor Modelo de Vendas</span>

Quando o treinamento do modelo estiver concluído, você poderá analisar o melhor modelo treinado pelo projeto de aprendizado automático.

1. Na página de **Visão Geral do Projeto de Aprendizado Automático**, observe o resumo do melhor modelo. Identifique o algoritmo utilizado e outras métricas importantes.

2. Selecione o modelo para ver mais detalhes, como métricas de desempenho, gráficos e insights.

## <span style="color:green">Implante e Teste o Modelo de Vendas</span>

Agora você pode implantar e testar o modelo de vendas treinado para prever as preferências do cliente em tempo real.

1. Na página do **Modelo do Melhor Modelo Treinado**, selecione **Implantar** e use a opção de **Serviço Web** para implantar o modelo com as configurações desejadas.

2. Aguarde a implantação do serviço. Isso pode levar alguns minutos.

3. Após a implantação ser bem-sucedida, você pode testar o serviço de vendas implantado utilizando dados de entrada simulados.

## <span style="color:green">Teste o Serviço de Vendas Implantado</span>

Agora você pode testar o serviço de vendas implantado para prever as preferências do cliente em tempo real.

1. No **Painel de Controle** da Plataforma de Vendas no Azure, selecione **Endpoints** e abra o endpoint do serviço de vendas implantado.

2. Na página do **Endpoint do Serviço em Tempo Real**, vá para a aba de **Teste**.

3. No Painel de **Dados de Entrada para Testar o Endpoint**, insira dados de entrada simulados e execute o teste.

4. Revise os resultados do teste, que incluem as previsões de preferências do cliente com base nos dados de entrada fornecidos.

## <span style="color:green">Limpeza</span>

Após concluir o exercício, lembre-se de limpar os recursos utilizados para evitar custos desnecessários.

1. No **Painel de Controle** da Plataforma de Vendas no Azure, exclua o endpoint do serviço de vendas implantado.

2. No Portal do Azure, exclua o grupo de recursos que contém os recursos da plataforma de vendas.

Agora você explorou com sucesso o uso do aprendizado automático para prever as preferências do cliente e otimizar as vendas de automóveis!
