# Como as atribuições de recursos direcionam o cronograma?
Se você não atribuir recursos a tarefas no projeto, o Project calculará o cronograma usando durações, dependências entre tarefas, restrições e informações do calendário do projeto e da tarefa. Se você atribuir recursos, as tarefas também serão agendadas de acordo com os calendários dos recursos e unidades de atribuição, permitindo um agendamento mais preciso.

> **Observação**: As tarefas agendadas manualmente não são afetadas pelos calendários de recursos. Quando um recurso for atribuído a uma tarefa agendada manualmente, o agendamento da tarefa não será alterado.

Uma atribuição é a associação de uma tarefa específica com um recurso específico que é responsável pela realização da tarefa. É possível atribuir mais de um recurso a uma tarefa. Recursos de trabalho, recursos materiais e recursos de custo podem ser atribuídos a tarefas. Diferentemente dos recursos de trabalho, a atribuição de recursos materiais ou de recursos de custo a uma tarefa não afeta o agendamento da tarefa.

Por exemplo, em seu projeto você tem uma tarefa chamada **Desenvolver especificações**. Você também tem um recurso de engenharia, Sílvio. Se você atribuir Sílvio à tarefa **Desenvolver especificações**, o agendamento dessa tarefa dependerá do calendário do recurso e das unidades de atribuição de Sílvio, além das informações da tarefa, como duração, dependências entre tarefas, restrições e calendários.

Além de agendar de acordo com as informações da tarefa, depois que você atribuir recursos às tarefas do projeto, o Project terá informações adicionais dos recursos e as atribuições para usar no cálculo das informações do cronograma, incluindo:

|Atribuição ou configuração do recurso| Explicação                      |
|-------------------------------------|---------------------------------|
|   **Trabalho**                      | A quantidade de trabalho ou trabalho de horas extras que o recurso está atribuído para realizar, e o modo como esse trabalho está distribuído ao longo do tempo. A distribuição do trabalho ao longo do tempo também pode ser afetada pelos contornos.|
|   **Unidades de atribuição   **   |   O número de unidades de atribuição para o recurso, ou seja, meio expediente, tempo integral ou múltiplos, na tarefa.|
|   **Tipo de tarefa**              |   O tipo de tarefa que afeta a forma como um cronograma será alterado se você revisar a atribuição existente. Os três tipos de tarefa são unidade fixa, duração fixa e trabalho fixo.|
|   **Controlado pelo esforço**     |   Se a tarefa é controlada pelo esforço. Se uma tarefa for controlada pelo esforço, conforme os recursos forem adicionados ou removidos na atribuição, o trabalho permanecerá constante para a tarefa e será redistribuído entre os recursos. Para tarefas de unidades fixas, por exemplo, um resultado será que, se mais recursos forem atribuídos uma duração menor será necessária para concluir a tarefa. Consulte as seções acima neste artigo para saber mais sobre a configuração de controle pelo empenho.|
|   **Calendários**                 |   Calendários de recursos. O Project agenda os recursos atribuídos com base nos períodos de trabalho e de folga em seus calendários de recursos.|
|   **Contornos do trabalho**       |   Os contornos do trabalho permitem ajustar precisamente quando os recursos trabalham em tarefas, como durante uma fase de aumento. No modo de exibição **Uso da Tarefa**, clique com o botão direito do mouse no nome do recurso atribuído a uma tarefa e selecione um padrão de trabalho predefinido na lista **Contorno do trabalho**. Depois de selecionar o padrão, você pode ajustar manualmente as horas na parte com divisão ao longo do tempo do modo de exibição de uso.|

Para atribuir recursos a tarefas, clique na guia **Recurso** e em **Atribuir Recursos**.