# Como as restrições nas tarefas afetam o cronograma?
As restrições permitem controlar a data de início ou de término de uma tarefa agendada automaticamente. Existem três tipos de restrições:

* As restrições flexíveis não têm datas específicas associadas a elas. A configuração dessas restrições permite iniciar as tarefas o mais cedo ou o mais tarde possível, com as tarefas terminando antes do final do projeto, dadas as outras restrições e dependências entre tarefas do cronograma.

* As restrições semiflexíveis exigem uma data associada que controla a data de início ou de término mais anterior ou mais posterior de uma tarefa. Essas restrições permitem que uma tarefa termine a qualquer momento, desde que respeite o prazo de início ou de término.

* As restrições inflexíveis exigem uma data associada que controla a data de início ou de término da tarefa. Essas restrições são úteis quando você precisa fazer o cronograma e considerar fatores externos, como a disponibilidade de equipamento ou recursos, datas limite, marcos de contratos, e datas de início e de término.

**Dica de gerenciamento de projetos** Em quase todos os casos, use a restrição OMBP. Com ela, o mecanismo de agendamento tem a maior flexibilidade para determinar a data de término ideal para o projeto.

Estas são duas formas de exibir instantaneamente as restrições em suas tarefas.

* Para revisar ou alterar a restrição em uma tarefa, clique com o botão direito do mouse na tarefa, clique em **Informações da Tarefa** e clique na guia **Avançado**. As informações de restrições se encontram nas caixas **Tipo de restrição** e **Data de restrição**.

* Se a restrição for diferente de OMBP ou OMTP, o tipo de restrição exibirá seu indicador gráfico associado na coluna Indicador de qualquer modo de exibição de planilha, como o gráfico de Gantt.

As restrições com flexibilidade de agendamento moderada restringirão o início ou o término de uma tarefa antes ou depois de uma data que você escolher. Por exemplo, uma tarefa com uma restrição NIAD (Não Iniciar Antes de) para 15 de junho e uma dependência término-a-início com outra tarefa poderá começar em 15 de junho, se sua predecessora termina até 15 de junho (ou depois, se sua predecessora terminar depois de 15 de junho). Porém, ela não pode ser agendada para antes de 15 de junho. Por exemplo, esse uso das restrições poderá ser apropriado se você tiver um alvará de execução da obra válido apenas para datas específicas. Nesse caso, deverão ser usadas as restrições NIAD ou NTDD.

Antes e depois de aplicar uma restrição.gif

1. Com a relação entre tarefas término-a-início padrão e uma restrição OMBP aplicada a essas tarefas, a tarefa sucessora (a segunda) é agendada para começar assim que a tarefa predecessora (a primeira) estiver agendada para ser concluída.

2. Com uma restrição NIAD aplicada, a tarefa sucessora não pode começar antes da data da restrição, mesmo que (como mostrado aqui) a tarefa predecessora seja concluída antes da data da restrição.

A tabela a seguir lista as restrições fornecidas no Project.

|   Tipo de restrição   |   Nome da restrição   |   Descrição                   |
|-----------------------|-----------------------|-------------------------------|
|   Flexível            |   O Mais Tarde Possível (OMTP)|   Agenda a tarefa o mais tarde possível, com seu final antes do final do projeto e sem atrasar as tarefas subsequentes. Essa é a restrição padrão para tarefas quando você agenda a partir da data de término do projeto. Com essa restrição, não insira uma data de início ou de término da tarefa.|
|   Flexível            |   O Mais Breve Possível (OMBP)|   Agenda a tarefa para começar o mais cedo possível. Essa é a restrição padrão para tarefas quando você agenda a partir da data de início do projeto. Com essa restrição, não insira uma data de início ou de término.|
|   Semiflexível        |   Não Iniciar Antes de (NIAD)|    Agenda a tarefa para iniciar em ou depois de uma data especificada. Use essa restrição para garantir que uma tarefa não comece antes de uma data especificada.|
|   Semiflexível        |   Não Terminar Antes de (NTAD)|   Agenda a tarefa para terminar em ou depois de uma data especificada. Use essa restrição para garantir que uma tarefa não termine antes de uma determinada data.|
|   Semiflexível        |   Não Iniciar Depois de (NIDD)|   Agenda a tarefa para iniciar em ou antes de uma data especificada. Use essa restrição para garantir que uma tarefa não comece depois de uma data especificada.|
|   Semiflexível        |   Não Terminar Depois de (NTDD)|  Agenda a tarefa para terminar em ou antes de uma data especificada. Use essa restrição para garantir que uma tarefa não termine depois de uma determinada data.|
|   Inflexível          |   Deve Terminar em (DTE)|     Agenda a tarefa para terminar em uma data especificada. Define as datas de término antecipado, agendado e o limite da data de término para a data digitada e ancora a tarefa no cronograma.|
|   Inflexível          |   Deve Iniciar em (DIE)|      Agenda a tarefa para começar em uma data especificada. Define as datas de início antecipado, agendado e limite da data de início para a data digitada e ancora a tarefa no cronograma.|


Por padrão, todas as tarefas de um projeto agendado a partir da data de início têm a restrição OMBP aplicada. De forma semelhante, por padrão, todas as tarefas de um projeto agendado a partir da data de término têm a restrição OMTP aplicada.

Em geral, as restrições inflexíveis substituem todas as dependências entre tarefas e restringem uma tarefa a uma data à sua escolha. Por exemplo, uma tarefa com uma restrição DIE para 30 de setembro e uma dependência término-a-início com outra tarefa sempre será agendada para 30 de setembro, independentemente de sua predecessora terminar antecipada ou atrasada. Você pode alterar esse comportamento. Clique em **Arquivo, Opções, Agendar** e marque a caixa de seleção **As tarefas sempre obedecem às suas datas de restrição.**