# Como o agendamento controlado pelo empenho afeta o cronograma?
Em todas as tarefas, depois que você atribui um recurso, a tarefa é agendada de acordo com a fórmula (presumindo que as tarefas sejam do tipo tarefa de unidades fixas padrão):

_Duration = Work / Units_

Para qualquer tarefa, você pode escolher que parte da equação o Project calcula definindo o tipo de tarefa. Quando você atribui ou remove pessoas de uma tarefa, o Project aumenta ou encurta a duração da tarefa com base no número de recursos atribuídos a ela, mas não altera o trabalho total da tarefa. Isso é chamado de agendamento controlado pelo esforço. Normalmente, essa configuração está desativada. Para ativá-la, clique em **Arquivo, Opções, Agendar** e marque a caixa de seleção **Novas tarefas são controladas pelo empenho.**

Embora o agendamento controlado pelo empenho possa funcionar na maioria dos cenários, talvez você queira que esse comportamento reflita de forma mais precisa o que acontece em uma tarefa específica quando recursos são adicionados ou removidos. Por exemplo, você pode querer ver o aumento total de trabalho conforme adiciona mais pessoas a uma determinada tarefa.

1. Clique com o botão direito do mouse em uma tarefa, clique em **Informações da Tarefa**  botão Expandir e clique na guia **Avançado**.

2. Desmarque a caixa de seleção **Controlada pelo empenho.**

> Observação: Você não pode remover o agendamento controlado pelo empenho de tarefas de trabalho fixo. As tarefas de trabalho fixo não têm valores de trabalho flexíveis e sempre são, portanto, controladas pelo empenho.

Ao trabalhar com o agendamento controlado pelo empenho, lembre-se do seguinte:

|   Dicas e truques     |   Explicação                                          |
|-----------------------|-------------------------------------------------------|
|   O controle pelo empenho não se aplica ao primeiro recurso atribuído|   Os cálculos controlados pelo empenho se aplicam apenas depois que os primeiros recursos são atribuídos à tarefa. Depois que os primeiros recursos são atribuídos, o valor do trabalho não mudam, pois novos recursos são atribuídos ou removidos da mesma tarefa.|
|   Lembre-se das tarefas de unidades fixas|    Se o tipo de tarefa atribuída for **Unidades Fixas**, a atribuição de recursos adicionais encurta a duração da tarefa.|
|   Lembre-se das tarefas de duração fixa   |   Se o tipo de tarefa atribuída for **Duração Fixa**, a atribuição de recursos adicionais diminui os valores de unidade individuais dos recursos.|
|   Lembre-se das tarefas de unidades fixas |   Se o tipo de tarefa atribuída for **Trabalho Fixo**, a atribuição de recursos adicionais encurta a duração da tarefa.|
|   Algumas tarefas podem ser definidas para serem controladas pelo empenho |   As tarefas resumo e os projetos inseridos não podem ser definidos como **Controlados pelo empenho.**|