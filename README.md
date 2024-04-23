# AIAzureBootcamp
Criando um modelo e testando no Azure Machine Learning
Passo a passo:

    Criação de um Azure Machine Learning Workspace:
        Acesse o portal do Azure em https://portal.azure.com e faça login com suas credenciais da Microsoft.
        Selecione "+ Criar um recurso", pesquise por "Machine Learning" e crie um novo recurso Azure Machine Learning com as configurações necessárias (assinatura, grupo de recursos, nome único, região, etc.).
        Aguarde a criação do espaço de trabalho e acesse o Azure Machine Learning Studio.

    Treinamento do Modelo com Automated Machine Learning:
        No Azure Machine Learning Studio, acesse a página Automated ML (na seção de Autoria).
        Crie um novo job Automated ML com as configurações específicas (nome do job, nome do experimento, descrição, tipo de tarefa, conjunto de dados, métrica principal, algoritmos permitidos, etc.).
        Envie o job de treinamento e aguarde a conclusão (pode demorar um pouco).

    Revisão do Melhor Modelo:
        Após a conclusão do job Automated ML, na aba Visão Geral, observe o resumo do melhor modelo treinado.
        Selecione o nome do algoritmo para ver detalhes adicionais.
        Na aba Métricas, observe os gráficos de desempenho do modelo.

    Implantação e Teste do Modelo:
        Na aba Modelo para o melhor modelo treinado, selecione "Implantar" e use a opção de serviço web.
        Defina as configurações de implantação (nome, descrição, tipo de computação, autenticação, etc.) e aguarde a conclusão da implantação.
        Após a implantação, acesse o endpoint do serviço web e use a opção de teste para enviar dados de entrada e receber a saída do modelo.

    Limpeza de Recursos:
        Se não pretende continuar a usar o serviço web, exclua o endpoint para evitar custos desnecessários.
        No Azure Machine Learning Studio, na aba Endpoints, selecione o endpoint e exclua-o.
        Se deseja evitar custos de armazenamento de dados, delete o Azure Machine Learning Workspace e os recursos associados.
