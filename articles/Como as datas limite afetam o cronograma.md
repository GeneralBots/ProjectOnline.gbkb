# Como as datas limite afetam o cronograma?
Em geral, as datas limite não afetam o agendamento de tarefas. Elas são usadas para indicar uma data-alvo que você não quer perder, sem exigir que você defina uma restrição da tarefa que possa afetar o agendamento se a tarefa predecessora for alterada. Uma tarefa com uma data limite é agendada da mesma forma que qualquer outra, mas quando uma tarefa termina depois de sua data limite, o Project exibe o indicador da tarefa notificando que a tarefa perdeu sua data limite.

Para revisar ou alterar a data limite de uma tarefa, clique com o botão direito do mouse na tarefa, clique em **Informações da Tarefa** e clique na guia **Avançado**. Use a caixa **Data Limite**.

As datas limite podem afetar a margem de atraso total de tarefas. Se você inserir uma data limite antes do final da margem de atraso total da tarefa, a margem de atraso total será recalculada usando a data limite, em vez do limite da data de término da tarefa. A tarefa se tornará crítica se a margem de atraso total atingir zero.

Você pode definir datas limite para tarefas resumo e também para tarefas individuais. Se a data limite da tarefa resumo entrar em conflito com qualquer uma das subtarefas, o indicador de data limite significará uma data limite perdida entre as subtarefas.

Mas as datas limite poderão afetar a forma como as tarefas são agendadas, se você definir uma data limite em uma tarefa com uma restrição OMTP (O Mais Tarde Possível). A tarefa é agendada para terminar na data limite, embora ela ainda possa terminar depois de sua data limite, se as predecessoras forem adiadas.