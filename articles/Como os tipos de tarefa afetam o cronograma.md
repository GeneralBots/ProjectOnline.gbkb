# Como os tipos de tarefa afetam o cronograma?
Os tipos de tarefa se aplicam apenas a tarefas agendadas automaticamente e têm três opções: unidades fixas, trabalho fixo e duração fixa. O Project examina o tipo de uma tarefa para determinar como a duração, o trabalho e as unidades se comportarão enquanto o Project agenda o projeto.

Cada um dos tipos de tarefa afeta o agendamento quando você edita um dos três elementos da seguinte maneira.

|   Em uma      |   Se você revisar as unidades|    Se você revisar a duração|  Se você revisar o trabalho|
|---------------|------------------------------|-----------------------------|----------------------------|
|   Tarefa de unidades fixas|   A duração é recalculada.|   O trabalho é recalculado.|  A duração é recalculada.|
|   Tarefa de trabalho fixo|    A duração é recalculada.|   As unidades são recalculadas.|  A duração é recalculada.|
|   Tarefa de duração fixa  |   O trabalho é recalculado.|  O trabalho é recalculado.    |  As unidades são recalculadas.|

* Para alterar um tipo de tarefa, clique duas vezes no nome da tarefa no gráfico de Gantt e clique na guia **Avançado**.

**Alguns exemplos**
Digamos que você tenha uma tarefa de unidades fixas, com 1 unidade de recurso de tempo integral disponível 8 horas por dia. Você define a tarefa com uma duração de 10 dias e 80 horas de trabalho.

* Se você descobrir que outro recurso de tempo integral pode auxiliar na tarefa, o Project recalculará a duração da tarefa. Agora a tarefa tem duas unidades atribuídas, com uma duração de 5 dias e 80 horas de trabalho.

* Se você descobrir que tem 8 dias para concluir a tarefa, em vez de 10, o Project recalculará o trabalho da tarefa. A tarefa tem agora uma duração de 8 dias, com 64 horas de trabalho e 1 unidade de recurso.

* Se você descobrir que a tarefa levará 20 horas de trabalho adicional, o Project recalculará a duração da tarefa. A tarefa tem agora 100 horas de trabalho, com uma duração de 12,5 dias e 1 unidade de recurso.

Agora, digamos que você transforme a mesma tarefa em uma tarefa de trabalho fixo. Isso significa que ela pode fazer apenas o trabalho que você especificar: nem mais, nem menos. Nesse exemplo, a tarefa tem 1 recurso de tempo integral disponível 8 horas por dia, com uma duração de 10 dias e 80 horas de trabalho.

* Se você descobrir que outro recurso de tempo integral pode auxiliar na tarefa, o Project recalculará a duração da tarefa. Agora a tarefa tem 2 unidades atribuídas, com uma duração de 5 dias e 80 horas de trabalho.

* Se você descobrir que tem 8 dias para concluir a tarefa, em vez de 10, o Project recalculará as unidades de recurso da tarefa. Para que a tarefa seja feita em 80 horas durante 8 dias, devem ser atribuídas 1,25 unidades de recurso. A unidade de recurso atribuída à tarefa no momento está alocada a 125%. Você precisa atribuir outro recurso para a alocação dos 25% adicionais.

* Se você descobrir que a tarefa levará 20 horas de trabalho adicional, o Project recalculará a duração da tarefa. A tarefa tem agora 100 horas de trabalho, com uma duração de 12,5 dias e 1 unidade de recurso.

Por fim, digamos que você transforme a mesma tarefa em uma tarefa de duração fixa. Isso significa que ela deve ser concluída na duração que você especificar. Novamente, Nesse exemplo, a tarefa tem 1 recurso de tempo integral disponível 8 horas por dia, com uma duração de 10 dias e 80 horas de trabalho.

* Se você descobrir que outro recurso pode auxiliar na tarefa, o Project recalculará o trabalho atribuído a cada recurso. Quando apenas 1 recurso estava atribuído à tarefa, esse recurso tinha 80 horas de trabalho para realizar. Quando você atribui outro recurso à tarefa, cada recurso tem 40 horas de trabalho para realizar ao longo da mesma duração de 10 dias, para um total de 80 horas de trabalho. Ao adicionar outra unidade de recurso, você também revisa a alocação das duas unidades para 50% cada, tornando as duas disponíveis para trabalhar 50% em outras tarefas.

* Se você descobrir que tem 8 dias para concluir a tarefa, em vez de 10, o Project recalculará o trabalho da tarefa. A tarefa tem agora uma duração de 8 dias, com 64 horas de trabalho e 1 unidade de recurso.

Se você descobrir que a tarefa levará 20 horas de trabalho adicional, o Project recalculará as unidades de recurso da tarefa, de forma que o trabalho adicional ainda possa ser concluído dentro da duração de 10 dias. A tarefa tem agora 100 horas de trabalho, com uma duração de 10 dias e 1,25 unidade de recurso. A unidade de recurso atribuída à tarefa no momento está alocada a 125%. Você precisa atribuir outro recurso para a alocação dos 25% adicionais.

> Observação: Como as atribuições de recursos de custo não têm valores para trabalho ou unidades, esses valores não serão recalculados quando a data de início ou a data de término de uma tarefa for modificada. As datas também nunca são recalculadas para uma atribuição de recurso de custo, pois não é possível modificar o trabalho ou as unidades.

Esta é uma tabela do que se deve lembrar sobre os tipos de tarefa.

|   Dicas e truques     |   Explicação                                                          |
|-----------------------|-----------------------------------------------------------------------|
|   Esteja atento às tarefas controladas pelo empenho| Se você clicar em Trabalho Fixo na lista Tipo de tarefa, não será possível alterar a configuração de Controlada pelo empenho da tarefa. As tarefas de trabalho fixo não têm valores de trabalho flexíveis e sempre são, portanto, controladas pelo empenho. Saiba mais sobre tarefas controladas pelo empenho posteriormente neste artigo.|
|   Adicione uma coluna para ajudar a alterar o tipo de tarefa|    Você pode exibir e alterar o tipo de cada tarefa diretamente em sua exibição inserindo o campo **Tipo**. Clique na coluna à direita de onde deseja inserir a nova coluna, clique no menu **Inserir** e em **Coluna**. Na lista **Nome do campo**, clique em **Tipo.**|
|   As tarefas resumo são sempre tarefas de duração fixa|  As tarefas de resumo são sempre do tipo de duração fixa, pois as datas de início e término de uma tarefa de resumo são determinadas por suas subtarefas.|
|   Use o recuo para a estrutura de tópicos, não para tipos de tarefa| Se desejar alterar a estrutura hierárquica de uma tarefa ou subtarefa como parte de uma estrutura de tópicos do projeto, você precisará recuar a tarefa ou recuá-la para a esquerda, em vez de alterar o tipo de tarefa ou adicionar uma data limite.|
|   Não confunda restrições de tarefas, como OMBP, com tipos de tarefa| Se desejar impor restrições sobre a forma como o Project calcula as datas de início e de término das tarefas, você precisará definir uma restrição de tarefa, em vez do tipo da tarefa.|
