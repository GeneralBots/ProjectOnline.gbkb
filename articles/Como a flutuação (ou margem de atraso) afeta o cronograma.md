# Como a flutuação (ou margem de atraso) afeta o cronograma?

A flutuação (também conhecida como margem de atraso) ajuda a localizar as tarefas que podem ser orçadas sem alterar a data de término do projeto. Talvez você queira exibir as tarefas que podem ser adiadas no momento sem afetar o caminho crítico (margem de atraso total) ou as tarefas que podem ser adiadas antes de afetar a tarefa à qual elas estão conectadas (margem de atraso permitida).

Estas são as duas maneiras de exibir a flutuação no cronograma.

* No gráfico de Gantt, clique em **Formatar** e marque a caixa de seleção **Margem de Atraso**. A flutuação é exibida como uma linha fina ligada ao final ou ao início das barras de Gantt.

Use o modo de exibição Gantt Detalhado. Clique em **Exibir, Outros Modos de Exibição, Mais Modos de Exibição, Gantt Detalhado** e em **Aplicar.**
Agora, de volta ao gráfico de Gantt, clique em **Tabelas** e em **Agendar**.

Estas são algumas coisas que se deve lembrar sobre a flutuação.

|   Dicas e truques |   Explicação                                                                 |
|-------------------|------------------------------------------------------------------------------|
|   Atenção às restrições inflexíveis| Se uma tarefa que está restrita a uma data tiver uma predecessora que termina tarde demais para que a sucessora comece na data especificada pela restrição, poderá ocorrer uma margem de atraso negativa. A margem de atraso negativa restringirá ainda mais a data de término do projeto.|
|   As datas limite alteram a margem de atraso total|   As datas limite podem afetar a margem de atraso total de tarefas. Se você inserir uma data limite antes do final da margem de atraso total da tarefa, a margem de atraso total será recalculada usando a data limite, em vez do limite da data de término da tarefa. A tarefa se tornará crítica se a margem de atraso total atingir zero.|