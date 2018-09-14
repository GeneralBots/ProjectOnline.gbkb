# Como a data de início do projeto afeta o cronograma?
Quando você adiciona uma nova tarefa a um cronograma, ela é automaticamente agendada para começar na data de início do projeto. Conforme as tarefas forem adicionadas ao cronograma e conectadas a outras tarefas, suas datas de início serão alteradas, e a tarefa que terminar por último definirá a data de término do projeto.

* Para localizar a data de início do projeto ou alterá-la, clique em **Projeto** e em **Informações do Projeto.**

Claro, haverá exceções. Por exemplo, as tarefas manualmente não se movem como as outras. Leia a seguir neste artigo para saber mais sobre a comparação entre o agendamento de tarefas manual e automático.

Antes e depois de criar uma dependência entre tarefas.gif

1. Quando você cria um novo projeto, primeiro insere a data de início do projeto. Quando você agenda um projeto a partir da data de início, todas as tarefas começam na data de início do projeto, a menos que você especifique de outra maneira.

2. Para tarefas agendadas manualmente e automaticamente, sem dependências entre tarefas ou restrições aplicadas, a duração do projeto é igual à duração da tarefa mais longa. Em outras palavras, a data de término do projeto é igual à data de término da tarefa mais longa.

3. As dependências de tarefas, como a dependência término-a-início entre a primeira e a segunda tarefas (como mostrado aqui) podem alterar a data de término do projeto.

Quase todos os projetos devem ser agendados a partir de uma data de início conhecida. Mesmo que você saiba a data em que um projeto deve ser concluído, o agendamento a partir de uma data de início dá a você o máximo de flexibilidade.

Contudo, talvez você queira agendar a partir de uma data de término quando:

* Você precisa determinar quando um projeto deve começar para que ele termine em uma data específica necessária.

* Você não tem certeza de quando o projeto começará (por exemplo, você está recebendo trabalho de outra fonte que pode se atrasar).

* Sua metodologia de gerenciamento de projetos exige que você agende a partir de uma data de término.

Ao trabalhar com um projeto agendado a partir de uma data de término, lembre-se das diferenças na forma como o Project trata algumas ações:

* Quando você insere uma tarefa agendada automaticamente, o Project atribui automaticamente a restrição OMTP (O Mais Tarde Possível) à data de término da tarefa. Você deve definir outras restrições somente quando necessário (clique com o botão direito do mouse em uma tarefa e clique em **Informações da Tarefa**).

* Se você arrastar uma barra de Gantt para alterar a data de término de uma tarefa, o Project atribuirá automaticamente uma restrição NTDD (Não Terminar Depois De) a uma tarefa agendada automaticamente.

* Se você alterar o projeto para ser agendado a partir de uma data de término e ele tiver sido agendado anteriormente a partir de uma data de início, você removerá todos os atrasos e as divisões de nivelamento das tarefas e atribuições que foram agendadas automaticamente. As tarefas agendadas manualmente não são afetadas.

* Se você usar o nivelamento automático para reduzir superalocações de recursos no projeto, o Project adicionará um atraso do nivelamento depois de uma tarefa, em vez de antes (para verificar as configurações do nivelamento, clique na guia **Recurso** e em **Nivelar Recurso**).