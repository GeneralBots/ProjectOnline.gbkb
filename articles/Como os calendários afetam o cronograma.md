# Como os calendários afetam o cronograma?
Os calendários determinam o período de trabalho e o período de folga padrão do projeto, como fins de semana e feriados.

> **Observação:** As datas de tarefas agendadas manualmente (se inseridas) não serão alteradas com base nas alterações dos calendários do projeto ou de recursos.

Os calendários do projeto são usados para determinar a disponibilidade de recursos, como os recursos atribuídos a tarefas são agendados e como as próprias tarefas são agendadas. Os calendários do projeto e da tarefa são usados no agendamento das tarefas e, se os recursos forem atribuídos a tarefas, os calendários de recursos também serão usados.

Os calendários sobrepõem as configurações uns dos outros da seguinte forma.

1. Quando você cria uma tarefa, o calendário do projeto agenda a tarefa.

2. Quando você adicionar um recurso a uma tarefa, o calendário do recurso controla o cronograma da tarefa.

3. Quando você adiciona um novo calendário de tarefa a uma tarefa e ajusta a configuração do calendário como **O agendamento ignora calendários de recursos** na caixa de Informações da Tarefa, o calendário da tarefa controla o cronograma e irá ignorar o cronograma de qualquer recurso atribuído para a tarefa.

Para trabalhar com calendários, clique em **Projeto** e em **Alterar Período Útil**.

|   Tipo de calendário      |   Descrição                                                       |
|---------------------------|-------------------------------------------------------------------|
|   Calendários base        |   São as bases para os outros tipos de calendários. Você também pode escolher um calendário base para ser o calendário do projeto e pode aplicar um calendário base a tarefas, como um calendário de tarefas ou como as horas padrão para um calendário de recursos. Você pode personalizar seu próprio calendário base usando qualquer um dos calendários base fornecidos.|
|                             |    O Project oferece três calendários base:
|                             |**O calendário Padrão**   O calendário Padrão é o calendário padrão para o projeto, e é a base para calendários de recursos. Esse calendário reflete um horário de trabalho tradicional: de segunda a sexta-feira, das 08h às 17h, com uma hora de intervalo.   
|                             |    **Calendário de 24 Horas**   O calendário 24 Horas refletirá um cronograma sem nenhum período de folga. O calendário 24 Horas pode ser usado quando os recursos e tarefas são agendados para turnos diferentes 24 horas ou quando os recursos de equipamento trabalham em uma tarefa continuamente. 
|                              |    **Calendários Turno da Noite**   O calendário Turno da Noite reflete um cronograma de turno da noite de segunda-feira à noite até sábado de manhã, das 23:00 às 08:00, com uma hora de intervalo.|
|   Calendários do projeto   |  Definem os períodos de trabalho e de folga padrão do projeto como um todo. Se os calendários de recursos ou de tarefas não forem usados, por padrão, as tarefas serão agendadas durante o período de trabalho no calendário do projeto.|
|   Calendários de recursos   | Geralmente são baseados no calendário do projeto no momento da criação do recurso. Você pode alterar o período de trabalho ou o período de folga para recursos específicos ou um conjunto de recursos, garantindo que eles sejam agendados somente quando estiverem disponíveis para trabalhar. Se você tiver alterado o período de trabalho ou de folga no calendário de um recurso e ele for atribuído a uma tarefa, a tarefa será agendada durante o período de trabalho no calendário do recurso. Isso também pode afetar a data de término da tarefa.  Os recursos podem herdar o período de folga do calendário base ou substituir esse período com as configurações do período de folga no calendário de recursos.|
|   Calendários de tarefas   |  Podem ser usados para definir os períodos de trabalho para tarefas fora dos períodos de trabalho do calendário de projetos. Os calendários de tarefas são criados da mesma forma que os outros calendários. Quando um calendário de tarefas é atribuído a uma tarefa e o recurso atribuído a ela tem períodos de trabalho diferentes em seu calendário de recursos, a tarefa é agendada para o período de trabalho sobreposto dos dois calendários. Mas você pode definir uma opção da tarefa para ignorar os calendários de recursos e agendar a tarefa por meio do período de folga do recurso. Se nenhum calendário de tarefa for especificado para uma tarefa, o calendário do projeto será usado para agendá-la.|